# unit

Speaks the value as a unit. Can be a number and unit or just a unit.

Units values include:

- 10 foot
- 10 ft
- 10ft
- foot
- ft
- 6'3" (depends on platform)


Some implementations of SSML converts units to singular or plural depending on the number.

```text
I would walk (500 mi)[unit]
```

---

### Speech Markdown
#### Short format
```text
n/a
```

#### Standard format
```text
I would walk (500 mi)[unit]
```

### Formatters
#### Plain Text
```text
I would walk 500 mi
```

#### Amazon Alexa SSML
```xml
<speak>
    I would walk <say-as interpret-as="unit">500 mi</say-as>
</speak>
```

#### Google Assistant SSML
```xml
<speak>
    I would walk <say-as interpret-as="unit">500 mi</say-as>
</speak>
```
