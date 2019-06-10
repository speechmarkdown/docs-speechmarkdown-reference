# What Is Speech Markdown?

Speech Markdown is the text-to-speech format for content authors.

## Benefits
- **Simplified.** Don't know the difference between prosody and phoneme? No problem. Simpler than Speech Synthesis Markup Language (SSML).

- **Converts to SSML or Text.** Just because voice platforms use SSML, doesn't mean that content authors must. Write content is Speech Markdown and convert it to SSML or plain text.

- **Supports Multiple Platforms.** Don't worry about how each platform supports (or does not support) the SSML specs [v1.0](https://www.w3.org/TR/2004/REC-speech-synthesis-20040907/) & [v1.1](https://www.w3.org/TR/speech-synthesis/). Use separate formatters to convert Speech Markdown to platform-specific SSML flavors such as [Amazon Alexa](https://developer.amazon.com/public/solutions/alexa/alexa-skills-kit/docs/speech-synthesis-markup-language-ssml-reference) and [Google Assistant](https://developers.google.com/actions/reference/ssml).


## Sample
Here is a quick sample that compares Speech Markdown and SSML.

Two common SSML elements are **&lt;break&gt;** and **&lt;emphasis&gt;**:

```xml
<speak>
    Step 1, take a deep breath. <break time="200ms"/>
    Step 2, exhale.
    Step 3, take a deep breath again. <break strength="weak"/>
    Step 4, exhale.

    This is <emphasis>an important</emphasis> announcement
    Are you <emphasis level="strong">listening?</emphasis>
</speak>
```

The sample above would be formatted in Speech Markdown as:

```
Step 1, take a deep breath. [200ms]
Step 2, exhale.
Step 3, take a deep breath again. [break:"weak"]
Step 4, exhale.

This is (an important)[emphasis] announcement
Are you ++listening?++
```

All elements have a standard format:
- `[break:"200ms"]`
- `[break:"weak"]`
- `(text)[emphasis]` or `(text)[emphasis:"moderate"]`
- `(text)[emphasis:"strong"]`

Some elements also have a short format:
- `[200ms]`
- `+text+`
- `++text++`
