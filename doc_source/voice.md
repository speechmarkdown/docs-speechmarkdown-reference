# voice

Sets the voice for the speech. The value is not validated. The formatter will use the value for a given voice if the platform supports it.

```
Using the default voice setting.

#[voice:"Kendra";lang:"en-US"]
Kendra from the US.

#[voice:"Brian";lang:"en-GB"]
Brian from the UK.

Why do you keep switching voices (from one)[voice:"Brian"] (to the other)[voice:"Kendra"]?
```

The `device` value removes any overrides, therefore using the device settings.

Currently, Amazon Alexa supports the following voices:
- Ivy (en-US)
- Joanna (en-US)
- Joey (en-US)
- Justin (en-US)
- Kendra (en-US)
- Kimberly (en-US)
- Matthew (en-US)
- Salli (en-US)
- Nicole (en-AU)
- Russell (en-AU)
- Amy (en-GB)
- Brian (en-GB)
- Emma (en-GB)
- Aditi (en-IN)
- Raveena (en-IN)
- Hans (de-DE)
- Marlene (de-DE)
- Vicki (de-DE)
- Conchita (es-ES)
- Enrique (es-ES)
- Carla (it-IT)
- Giorgio (it-IT)
- Mizuki (ja-JP)
- Takumi (ja-JP)
- Celine (fr-FR)
- Lea (fr-FR)
- Mathieu (fr-FR)


---
## modifier

You can use `voice` as a modifier for a word or phrase.

### Speech Markdown
#### Short format
```
n/a
```

#### Standard format
```
Why do you keep switching voices (from one)[voice:"Brian"] (to the other)[voice:"Kendra"]?
```

### Formatters
#### Plain Text
```
Why do you keep switching voices from one to the other?
```

#### Amazon Alexa SSML
```xml
<speak>
Why do you keep switching voices <voice name="Brian">from one</voice> <voice name="Kendra">to the other</voice>?
</speak>
```

#### Google Assistant SSML
```xml
<speak>
Why do you keep switching voices from one to the other?
</speak>
```

---
## section

You can use `voice` in a section.

### Speech Markdown
#### Short format
```
n/a
```

#### Standard format
```
#[voice:"Brian";lang:"en-GB"]
Brian from the UK.
```

### Formatters
#### Plain Text
```
Brian from the UK.
```

#### Amazon Alexa SSML
```xml
<speak>
    <voice name="Brian"><lang xml:lang="en-GB">Brian from the UK.</lang></voice>
</speak>
```

#### Google Assistant SSML
```xml
<speak>
Brian from the UK.
</speak>
```