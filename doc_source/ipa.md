# ipa

Provides a phonemic/phonetic pronunciation for the contained text using the International Phonetic Alphabet (IPA).

```
You say, (pecan)[ipa:"pɪˈkɑːn"].
I say, (pecan)[/ˈpi.kæn/].
```

---

### Speech Markdown
#### Short format
```
I say, (pecan)[/ˈpi.kæn/].
```

#### Standard format
```
I say, (pecan)[ipa:"ˈpi.kæn"].
```

### Formatters
#### Plain Text
```
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
