# spell-out

Speaks a number or text as individual characters.

The same as

- [digits](../syntax/digits) (numbers only)
- [characters](../syntax/characters)
- [verbatim](../syntax/verbatim)

```text
Countdown: (321)[spell-out]

The word is spelled: (park)[spell-out]

(801)[digits] is the same as (801)[characters] which is the same as (801)[spell-out] and (801)[verbatim].

(dog)[characters] is the same as (dog)[spell-out] and (dog)[verbatim]
```

---

### Speech Markdown
#### Short format
```text
n/a
```

#### Standard format
```text
Countdown: (321)[spell-out].
The word is spelled: (park)[spell-out].
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
    Countdown:: <say-as interpret-as="spell-out">321</say-as>.
    The word is spelled: <say-as interpret-as="spell-out">park</say-as>.
</speak>
```

#### Google Assistant SSML
```xml
<speak>
    Countdown:: <say-as interpret-as="spell-out">321</say-as>.
    The word is spelled: <say-as interpret-as="spell-out">park</say-as>.
</speak>
```
