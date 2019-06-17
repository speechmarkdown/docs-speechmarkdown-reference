# volume / vol

Modify the volume of the speech.

```text
Normal volume for the first sentence.
(Louder volume for the second sentence)[volume:"x-loud"].

Volume modifier (can be abbreviated)[vol:"soft"].

I can combine (multiple values)[pitch:"low";rate:"slow";volume:"loud";voice:"Brian"] at once.
```

---

Possible values:

- silent
- x-soft
- soft
- medium (default rate)
- loud
- x-loud


### Speech Markdown
#### Short format
```text
n/a
```

#### Standard format
```text
Normal volume for the first sentence.
(Louder volume for the second sentence)[volume:"x-loud"].
```

### Formatters
#### Plain Text
```text
Normal volume for the first sentence.
Louder volume for the second sentence.
```

#### Amazon Alexa SSML
```xml
<speak>
    Normal volume for the first sentence.
    <prosody volume="x-loud">Louder volume for the second sentence</prosody>.
</speak>
```

#### Google Assistant SSML
```xml
<speak>
    Normal volume for the first sentence.
    <prosody volume="x-loud">Louder volume for the second sentence</prosody>.
</speak>
```
