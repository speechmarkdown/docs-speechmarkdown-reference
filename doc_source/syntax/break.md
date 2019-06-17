# break

A pause in speech.

```text
Step 1, take a deep breath. [200ms]
Step 2, exhale.
Step 3, take a deep breath again. [break:"weak"]
Step 4, exhale.
```
---
## time

Set break length in seconds or milliseconds:

- 250ms
- 0.5s
- 3s
- 10s
- 10000ms


### Speech Markdown
#### Short format
```text
A pause [250ms] then continue.
```

#### Standard format
```text
A pause [break:"250ms"] then continue.
```

### Formatters
#### Plain Text
```text
A pause then continue.
```

#### Amazon Alexa SSML
```xml
<speak>
A pause <break time="250ms"/> then continue.
</speak>
```

#### Google Assistant SSML
```xml
<speak>
A pause <break time="250ms"/> then continue.
</speak>
```

---

## strength

Set break length by relative terms:

- none
- x-weak
- weak
- medium
- strong
- x-strong


### Speech Markdown
#### Short format
```text
n/a
```

#### Standard format
```text
A pause [break:"weak"] then continue.
```

### Formatters
#### Plain Text
```text
A pause then continue.
```

#### Amazon Alexa SSML
```xml
<speak>
A pause <break strength="weak"/> then continue.
</speak>
```

#### Google Assistant SSML
```xml
<speak>
A pause <break strength="weak"/> then continue.
</speak>
```