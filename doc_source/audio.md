# audio

Plays short, pre-recorded audio.

```
!["https://intro.mp3"]
Welcome back.
```

---
## MP3

Both Amazon Alexa and Google Assistant support the MP3 format for audio. Consult documentation for each platform for supported duration, bit rate, sample rate, and hosting info.

No validation is done on the passed URL.


### Speech Markdown
#### Short format
```
n/a
```

#### Standard format
```
!["https://intro.mp3"]
Welcome back.
```

### Formatters
#### Plain Text
```
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
    <audio src="https://intro.mp3"/>
    Welcome back.
</speak>
```
