# digits

Speaks a number as individual digits.

The same as
- [characters](characters.md)
- [spell-out](spell-out.md)
- [verbatim](verbatim.md)

```
Countdown: (321)[digits]

(801)[digits] is the same as (801)[characters] which is the same as (801)[spell-out] and (801)[verbatim].
```

---

### Speech Markdown
#### Short format
```
n/a
```

#### Standard format
```
Countdown: (321)[digits]
```

### Formatters
#### Plain Text
```
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
