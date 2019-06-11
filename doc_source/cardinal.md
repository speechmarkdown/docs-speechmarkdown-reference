# cardinal

Speaks a number as a cardinal: one, twenty, twelve thousand three hundred forty five, etc.

The same as [number](number.md).

```
One, two, (3)[cardinal].

Your balance is: (12345)[cardinal].

(801)[cardinal] is the same as (801)[number]
```

---

### Speech Markdown
#### Short format
```
n/a
```

#### Standard format
```
Your balance is: (12345)[cardinal].
```

### Formatters
#### Plain Text
```
Your balance is: 12345.
```

#### Amazon Alexa SSML
```xml
<speak>
    Your balance is: <say-as interpret-as="cardinal">12345</say-as>.
</speak>
```

#### Google Assistant SSML
```xml
<speak>
    Your balance is: <say-as interpret-as="cardinal">12345</say-as>.
</speak>
```
