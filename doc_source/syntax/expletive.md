# expletive / bleep

"Bleep" out the content

```text
You can't say (word)[bleep] on TV.
You said (word)[bleep] and (word)[expletive] at school.
```

---

### Speech Markdown
#### Short format
```text
n/a
```

#### Standard format
```text
You said (word)[bleep] and (word)[expletive] at school.
```

### Formatters
#### Plain Text
```text
You said word and word at school.
```

#### Amazon Alexa SSML
Since Amazon Alexa doesn't support `bleep` it is replaced with `expletive`.
```xml
<speak>
    You said <say-as interpret-as="expletive">word</say-as> and <say-as interpret-as="expletive">word</say-as> at school.
</speak>
```

#### Google Assistant SSML
```xml
<speak>
    You said <say-as interpret-as="bleep">word</say-as> and <say-as interpret-as="expletive">word</say-as> at school.
</speak>
```
