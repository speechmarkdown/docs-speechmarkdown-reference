# pitch

Raise or lower the tone (pitch) of the speech.

```
I can speak with my normal pitch, (but also with a much higher pitch)[pitch:"x-high"].

I can combine (multiple values)[pitch:"low";rate:"slow";volume:"loud";voice:"Brian"] at once.
```

---

Possible values:
- x-low
- low
- medium (default pitch)
- high
- x-high


### Speech Markdown
#### Short format
```
n/a
```

#### Standard format
```
I can speak with my normal pitch, (but also with a much higher pitch)[pitch:"x-high"].
```

### Formatters
#### Plain Text
```
I can speak with my normal pitch, but also with a much higher pitch.
```

#### Amazon Alexa SSML
```xml
<speak>
    I can speak with my normal pitch,
    <prosody pitch="x-high"> but also with a much higher pitch </prosody>.
</speak>
```

#### Google Assistant SSML
```xml
<speak>
    I can speak with my normal pitch,
    <prosody pitch="x-high"> but also with a much higher pitch </prosody>.
</speak>
```
