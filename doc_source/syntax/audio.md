# audio

Plays short, pre-recorded audio.

```text
!["https://intro.mp3"]
Welcome back.
```

An optional caption is supported:

```text
!(our intro)["https://intro.mp3"]
```

---
## MP3

Both Amazon Alexa and Google Assistant support the MP3 format for audio. Consult documentation for each platform for supported duration, bit rate, sample rate, and hosting info.

No validation is done on the passed URL.


### Speech Markdown
#### Short format
```text
n/a
```

#### Standard format
```text
!(optional caption)["https://intro.mp3"]
Welcome back.
```

### Formatters
#### Plain Text
```text
Welcome back.
```

#### Amazon Alexa SSML
```xml
<speak>
    <audio src="https://intro.mp3"/>
    Welcome back.
</speak>
```

#### Google Assistant SSML
```xml
<speak>
    <audio src="https://intro.mp3">
        <desc>optional caption</desc>
    </audio>
    Welcome back.
</speak>
```
