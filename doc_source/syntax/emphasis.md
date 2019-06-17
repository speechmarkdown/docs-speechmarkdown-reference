# emphasis

Add or remove emphasis from a word or phrase.

```text
A ++strong++ level
A +moderate+ level
A ~none~ level
A -reduced- level


A (strong)[emphasis:"strong"] level

A (moderate)[emphasis] level                //same
A (moderate)[emphasis:"moderate"] level     //same

A (none)[emphasis:"none"] level

A (reduced)[emphasis:"reduced"] level
```

Set break length in seconds or milliseconds:

- strong
- moderate (default)
- none
- reduced


### Speech Markdown
#### Short format
```text
A ++strong++ level
A +moderate+ level
A ~none~ level
A -reduced- level
```

#### Standard format
```text
A (strong)[emphasis:"strong"] level

A (moderate)[emphasis] level                //same
A (moderate)[emphasis:"moderate"] level     //same

A (none)[emphasis:"none"] level

A (reduced)[emphasis:"reduced"] level
```

### Formatters
#### Plain Text
```text
A strong level
A moderate level
A none level
A reduced level
```

#### Amazon Alexa SSML
```xml
<speak>
A <emphasis level="strong">strong</emphasis> level

A <emphasis level="moderate">moderate</emphasis> level

A <emphasis level="none">none</emphasis> level

A <emphasis level="reduced">reduced</emphasis> level
</speak>
```

#### Google Assistant SSML
```xml
<speak>
A <emphasis level="strong">strong</emphasis> level

A <emphasis level="moderate">moderate</emphasis> level

A <emphasis level="none">none</emphasis> level

A <emphasis level="reduced">reduced</emphasis> level
</speak>
```