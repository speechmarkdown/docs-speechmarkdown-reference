# ipa

Provides a phonemic/phonetic pronunciation for the contained text using the International Phonetic Alphabet (IPA).

```text
You say, (pecan)[ipa:"pɪˈkɑːn"].
I say, (pecan)[/ˈpi.kæn/].
```

---

### Speech Markdown
#### Short format
```text
I say, (pecan)[/ˈpi.kæn/].
```

#### Standard format
```text
I say, (pecan)[ipa:"ˈpi.kæn"].
```

### Formatters
#### Plain Text
```text
I say, pecan.
```

#### Amazon Alexa SSML
```xml
<speak>
    I say, <phoneme alphabet="ipa" ph="ˈpi.kæn">pecan</phoneme>.
</speak>
```

#### Google Assistant SSML
Google does not support the `<phoneme>` tag. Yet.

```xml
I say, pecan.
```
