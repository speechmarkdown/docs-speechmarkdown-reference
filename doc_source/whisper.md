# whisper

Speak text in a whispered voice.

```
I want to tell you a secret.
(I am not a real human.)[whisper]
Can you believe it?
```

---

### Speech Markdown
#### Short format
```
n/a
```

#### Standard format
```
(I am not a real human.)[whisper]
```

### Formatters
#### Plain Text
```
I am not a real human.
```

#### Amazon Alexa SSML
```xml
<speak>
    <amazon:effect name="whispered">I am not a real human.</amazon:effect>.
</speak>
```

#### Google Assistant SSML

Since Google Assistant doesn't have a whisper effect, through a configuration setting, you can either ignore the tag:

```xml
<speak>
    I am not a real human.
</speak>
```

or use an equivalent:

```xml
<speak>
    <prosody volume="x-soft" rate="slow">I am not a real human.</prosody>
</speak>
```

