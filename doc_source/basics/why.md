# Why Speech Markdown?

Here are some of the various reasons why Speech Markdown was created:

---

## 1. Shorter, simpler syntax
Instead of longer SSML:

```xml
<speak>
    A pause <break time="1s"/> then continue.
</speak>
```

Use more concise Speech Markdown:

```text
A pause [1s] then continue.
```

---

## 2. Convert to plain text
Use a plain text formatter and convert Speech Markdown:

```text
This is (an important)[emphasis] announcement
Are you ++listening?++
```

to plain text:

```text
This is an important announcement
Are you listening?
```

---

## 3. Convert to SSML

Use platform-specific formatters to convert Speech Markdown:

```text
Are you ++listening?++
```

to SSML for a given platform:

### Amazon Alexa

```xml
<speak>
    Are you <emphasis level="strong">listening?</emphasis>
</speak>
```

### Google Assistant

```xml
<speak>
    Are you <emphasis level="strong">listening?</emphasis>
</speak>

```

---

## 4. Extend with additional formatters
In addition to formatters for:

- Plain text
- Amazon Alexa
- Google Assistant

Formatters can be created for other platforms:

- Microsoft Cortana
- Amazon Polly
- IBM Watson
- and more

---

## 5. If markdown not supported by a platform, it is ignored
A platform's implementation of W3C standard SSML may not be complete and could differ from another platform.

One such example is the SSML `<phoneme>` tag that Amazon Alexa supports and Google Assistant does not.

When you use the `ipa` modifier in Speech Markdown:

```text
You say, (pecan)[ipa:"pɪˈkɑːn"].
I say, (pecan)[ipa:"ˈpi.kæn"].
```

The formatter will render in Amazon Alexa SSML:
```xml
<speak>
    You say, <phoneme alphabet="ipa" ph="pɪˈkɑːn">pecan</phoneme>.
    I say, <phoneme alphabet="ipa" ph="ˈpi.kæn">pecan</phoneme>.
</speak>
```

But the formatter will ignore it in Google Assistant SSML:

```xml
<speak>
    You say, pecan.
    I say, pecan.
</speak>
```


---

## 6. Platform-specific elements ignored by other platforms
Some Speech Markdown:

```text
(I am not a real human.)[whisper]
```

will be converted to a specific flavor of SSML using platform-specific formatters:

### Amazon Alexa

```xml
<speak>
    <amazon:effect name="whispered">I am not a real human.</amazon:effect>.
</speak>

```

### Google Assistant

```xml
<speak>
    I am not a real human.
</speak>

```

---

## 7. Platform-specific element substitution
Formatters can be configured to choose a similar substitution for platform-specific elements.

Some Speech Markdown:

```text
(I am not a real human.)[whisper]
```

will be converted to a specific flavor of SSML using platform-specific formatters:

### Amazon Alexa

```xml
<speak>
    <amazon:effect name="whispered">I am not a real human.</amazon:effect>.
</speak>

```

and pick a close substitution if a given tag is not supported:
### Google Assistant

```xml
<speak>
    <prosody volume="x-soft" rate="slow">I am not a real human.</prosody>
</speak>

```
---

## 8. Multiple Speech Markdown modifiers
When using multiple SSML tags on a single text block, the modified text can get lost in the nesting:

```xml
<speak>
    My favorite chemical element is <prosody volume="x-loud" rate="slow" pitch="low"><sub alias="aluminum">Al</sub></prosody>.
</speak>
```

Speech Markdown keeps the modified text together with the modifiers after:

```text
My favorite chemical element is (Al)[sub:"aluminum";volume:"x-loud";rate:"slow";pitch:"low"]
```
---


