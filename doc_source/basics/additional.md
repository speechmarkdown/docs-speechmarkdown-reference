# Additional Considerations

## Quotes
The value in the standard format Speech Markdown is always quoted. Either single or double quotes can be used:

```text
(some text)[emphasis:"strong"]  //OK
(some text)[emphasis:'strong']  //OK
```
---
## Paragraphs

Leaving an empty line between text content indicates paragraphs:

```text
This sentence makes up the first paragraph.

And this sentence is the second.
```

It is up to the configuration of the formatter that determines if the paragraph SSML tag `<p>` is rendered.

### Formatter - Render SSML &lt;p&gt;
```xml
<speak>
<p>This sentence makes up the first paragraph.</p>

<p>And this sentence is the second.</p>
</speak>
```

### Formatter - Don't render SSML &lt;p&gt;

```xml
<speak>
This sentence makes up the first paragraph.

And this sentence is the second.
</speak>
```
---
## Sentences
Speech Markdown does not require that sentences be identified. Therefore, formatters will typically NOT render the sentence SSML tag `<s>`.

---
## Order in Sections
The order of modifiers in sections is not important. When rendered the formatter will always render the `voice` modifier before the `lang` modifier.

These are the same:

```text
#[voice:"Joey";lang:"fr-FR";]
#[lang:"fr-FR";voice:"Joey"]
```

---
## Modifier order
In Speech Markdown, the order of `key:"value";` pairs is not important.

All the following are the same:

```text
(Al)[sub:"aluminum";volume:"x-loud";rate:"slow";pitch:"low"]
(Al)[volume:"x-loud";sub:"aluminum";pitch:"low";rate:"slow";]
(Al)[volume:"x-loud";rate:"slow";pitch:"low";sub:"aluminum";]
```
Because multiple modifiers can be rendered as a single SSML tag, the formatter is responsible for grouping them together.

The above sample includes the `sub` modifier which would be rendered in SSML as nested tags. Regardless of the order of the modifiers, the `<sub>` tag will always be innermost. This is also the responsibility of the formatter.

The same goes for the `ipa` modifier as it renders to SSML as `<phoneme alphabet="ipa"...>`.

---
## Modifier semi-colons
Semi-colons are only required when there are two or more modifiers. The trailing semi-colon is optional:

```text
(Al)[sub:"aluminum"]
(Al)[sub:"aluminum;"]

(text)[volume:"x-loud";pitch:"low";rate:"slow"]
(text)[volume:"x-loud";pitch:"low";rate:"slow";]
```

## Included SSML
If SSML is included in a Speech Markdown file, it is not processed. It should be in its own stand-alone paragraph.

```text
This is the (first)[emphasis] paragraph with Speech Markdown.

Are you <emphasis level="strong">listening?</emphasis>

This is the (last)[volume:"x-loud"] paragraph. The previous paragraph had SSML.
```
