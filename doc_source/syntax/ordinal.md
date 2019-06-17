# ordinal

Speaks a number as an ordinal: first, second, third, etc.

```text
The others came in 2nd and (3)[ordinal].

Your rank is (123)[ordinal].
```

---

### Speech Markdown
#### Short format
```text
n/a
```

#### Standard format
```text
The others came in 2nd and (3)[ordinal].
```

### Formatters
#### Plain Text
```text
The others came in 2nd and 3.
```

#### Amazon Alexa SSML
```xml
<speak>
    The others came in 2nd and <say-as interpret-as="ordinal">3</say-as>.
</speak>
```

#### Google Assistant SSML
```xml
<speak>
    The others came in 2nd and <say-as interpret-as="ordinal">3</say-as>.
</speak>
```
