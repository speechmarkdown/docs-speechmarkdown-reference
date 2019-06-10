# rate

Modify the rate of the speech.

```
When I wake up, (I speak quite slowly)[rate:"x-slow"].

I can combine (multiple values)[pitch:"low";rate:"slow";volume:"loud";voice:"Brian"] at once.
```

---

Possible values:
- x-slow
- slow
- medium (default rate)
- fast
- x-fast


### Speech Markdown
#### Short format
```
n/a
```

#### Standard format
```
When I wake up, (I speak quite slowly)[rate:"x-slow"].
```

### Formatters
#### Plain Text
```
I can speak with my normal pitch, but also with a much higher pitch.
```

#### Amazon Alexa SSML
```xml
<speak>
    When I wake up, <prosody rate="x-slow">I speak quite slowly</prosody>.
</speak>
```

#### Google Assistant SSML
```xml
<speak>
    When I wake up, <prosody rate="x-slow">I speak quite slowly</prosody>.
</speak>
```
