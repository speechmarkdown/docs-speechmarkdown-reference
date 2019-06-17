# sub

Substitute one word or phrase with a different word or phrase. Often used to expand/clarify abbreviations.

```text
My favorite chemical element is (Al)[sub:"aluminum"],
but Al prefers (Mg)["magnesium"].
```

---

### Speech Markdown
#### Short format
```text
The element is (Al)["aluminum"].
```

#### Standard format
```text
The element is (Al)[sub:"aluminum"].
```

### Formatters
#### Plain Text
```text
The element is Al.
```

#### Amazon Alexa SSML
```xml
<speak>
    The element is <sub alias="aluminum">Al</sub>.
</speak>
```

#### Google Assistant SSML
```xml
<speak>
    The element is <sub alias="aluminum">Al</sub>.
</speak>
```
