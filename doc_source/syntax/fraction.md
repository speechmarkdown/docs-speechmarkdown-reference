# fraction

Speaks the value as a fraction.


```text
Add (2/3)[fraction] cup of milk.
Add (1+1/2)[fraction] cups of flour.
```

---

### Speech Markdown
#### Short format
```text
n/a
```

#### Standard format
```text
Add (2/3)[fraction] cup of milk.
Add (1+1/2)[fraction] cups of flour.
```

### Formatters
#### Plain Text
```text
Add 2/3 cup of milk.
Add 1+1/2 cup of flour.
```

#### Amazon Alexa SSML
```xml
<speak>
    Add <say-as interpret-as="fraction">2/3</say-as> cup of milk.
    Add <say-as interpret-as="fraction">1+1/2</say-as> cups of flour.
</speak>
```

#### Google Assistant SSML
```xml
<speak>
    Add <say-as interpret-as="fraction">2/3</say-as> cup of milk.
    Add <say-as interpret-as="fraction">1+1/2</say-as> cups of flour.
</speak>
```
