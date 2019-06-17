# phone / telephone

Speak the number/value as a 7-digit or 10-digit telephone number.

The key, `phone` is a shortened form of `telephone` for convenience.

```text
My number is NOT (8675309)[phone].              // same
My number is NOT (8675309)[telephone].          // same
My number is NOT (8675309)[phone:"1"].          // same
My number is NOT (8675309)[telephone:"1"].      // same

The number is ((888) 555-1212)[phone].

```
Some implementations of SSML need a country code set as a `format` attribute. If no format is included, the default is "1".

---

### Speech Markdown
#### Short format
```text
n/a
```

#### Standard format
```text
The number is ((888) 555-1212)[phone].
```

### Formatters
#### Plain Text
```text
The number is (888) 555-1212.
```

#### Amazon Alexa SSML
The Alexa SSML formatter omits the `format` attribute.
```xml
<speak>
    The number is <say-as interpret-as="telephone">(888) 555-1212</say-as>.
</speak>
```

#### Google Assistant SSML
```xml
<speak>
    The number is <say-as interpret-as="telephone" format="1">(888) 555-1212</say-as>.
</speak>
```
