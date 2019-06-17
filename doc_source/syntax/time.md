# time

Speak the value as a time.

```text
The time is (2:30pm)[time:"hms12"].
The time is (2:30pm)[time:"hms24"].
```
Some implementations of SSML need a value the `format` attribute:

- hms12
- hms24


---

### Speech Markdown
#### Short format
```text
n/a
```

#### Standard format
```text
The time is (2:30pm)[time:"hms12"].
```

### Formatters
#### Plain Text
```text
The time is 2:30pm.
```

#### Amazon Alexa SSML
The Alexa SSML formatter omits the `format` attribute.
```xml
<speak>
    The time is <say-as interpret-as="time" format="hms12">2:30pm</say-as>.
</speak>
```

#### Google Assistant SSML
```xml
<speak>
    The time is <say-as interpret-as="time" format="hms12">2:30pm</say-as>.
</speak>
```
