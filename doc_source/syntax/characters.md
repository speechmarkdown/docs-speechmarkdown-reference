# characters

Speaks a number or text as individual characters.

```text
Countdown: (321)[characters]

The word is spelled: (park)[characters]
```

---

### Speech Markdown
#### Short format
```text
n/a
```

#### Standard format
```text
Countdown: (321)[characters].
The word is spelled: (park)[characters].
```

### Formatters
#### Plain Text
```text
Countdown: 321
The word is spelled: park.
```

#### Amazon Alexa SSML
```xml
<speak>
    Countdown:: <say-as interpret-as="characters">321</say-as>.
    The word is spelled: <say-as interpret-as="characters">park</say-as>.
</speak>
```

#### Google Assistant SSML
```xml
<speak>
    Countdown:: <say-as interpret-as="characters">321</say-as>.
    The word is spelled: <say-as interpret-as="characters">park</say-as>.
</speak>
```
