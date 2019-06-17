# address

Speaks the value as a street address.

```text
I'm at (150th CT NE, Redmond, WA)[address].
```

---

### Speech Markdown
#### Short format
```text
n/a
```

#### Standard format
```text
I'm at (150th CT NE, Redmond, WA)[address].
```

### Formatters
#### Plain Text
```text
I'm at 150th CT NE, Redmond, WA.
```

#### Amazon Alexa SSML
```xml
<speak>
    I'm at <say-as interpret-as="address">150th CT NE, Redmond, WA</say-as>.
</speak>
```

#### Google Assistant SSML
```xml
<speak>
    I'm at 150th CT NE, Redmond, WA.
</speak>
```
