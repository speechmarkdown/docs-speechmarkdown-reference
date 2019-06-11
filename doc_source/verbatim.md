# verbatim

Speaks a number or text as individual characters.

The same as
- [digits](digits.md) (numbers only)
- [characters](characters.md)
- [spell-out](spell-out.md)

```
Countdown: (321)[verbatim]

The word is spelled: (park)[verbatim]

(801)[digits] is the same as (801)[characters] which is the same as (801)[spell-out] and (801)[verbatim].

(dog)[characters] is the same as (dog)[spell-out] and (dog)[verbatim]
```

---

### Speech Markdown
#### Short format
```
n/a
```

#### Standard format
```
Countdown: (321)[verbatim].
The word is spelled: (park)[verbatim].
```

### Formatters
#### Plain Text
```
Countdown: 321
The word is spelled: park.
```

#### Amazon Alexa SSML

The `verbatim` modifier is not supported by Amazon Alexa, so an alternate is used:
```xml
<speak>
    Countdown:: <say-as interpret-as="characters">321</say-as>.
    The word is spelled: <say-as interpret-as="characters">park</say-as>.
</speak>
```

#### Google Assistant SSML
```xml
<speak>
    Countdown:: <say-as interpret-as="verbatim">321</say-as>.
    The word is spelled: <say-as interpret-as="verbatim">park</say-as>.
</speak>
```
