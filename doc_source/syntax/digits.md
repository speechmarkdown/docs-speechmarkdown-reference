# digits

Speaks a number as individual digits.

The same as

- [characters](../syntax/characters)
- [spell-out](../syntax/spell-out)
- [verbatim](../syntax/verbatim)

```text
Countdown: (321)[digits]

(801)[digits] is the same as (801)[characters] which is the same as (801)[spell-out] and (801)[verbatim].
```

---

### Speech Markdown
#### Short format
```text
n/a
```

#### Standard format
```text
Countdown: (321)[digits]
```

### Formatters
#### Plain Text
```text
Countdown: 321
```

#### Amazon Alexa SSML
```xml
<speak>
    Countdown:: <say-as interpret-as="digits">321</say-as>.
</speak>
```

#### Google Assistant SSML
```xml
<speak>
    Countdown:: <say-as interpret-as="digits">321</say-as>.
</speak>
```
