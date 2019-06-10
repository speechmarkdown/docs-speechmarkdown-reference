# lang

Sets the language. Words and phrases in other languages usually sound better with the `lang` tag.

```
Using the default language setting.

#[voice:"Kendra";lang:"en-US"]
Kendra from the US.

#[voice:"Brian";lang:"en-GB"]
Brian from the UK.

In Paris, they pronounce it (Paris)[lang:"fr-FR"].
```
---
## modifier

You can use `lang` as a modifier for a word or phrase.

### Speech Markdown
#### Short format
```
n/a
```

#### Standard format
```
In Paris, they pronounce it (Paris)[lang:"fr-FR"].
```

### Formatters
#### Plain Text
```
In Paris, they pronounce it Paris.
```

#### Amazon Alexa SSML
```xml
<speak>
    In Paris, they pronounce it <lang xml:lang="fr-FR">Paris</lang>
</speak>
```

#### Google Assistant SSML
```xml
<speak>
In Paris, they pronounce it Paris.
</speak>
```

---
## section

You can use `lang` in a section.

### Speech Markdown
#### Short format
```
n/a
```

#### Standard format
```
#[voice:"Brian";lang:"en-GB"]
Brian from the UK.
```

### Formatters
#### Plain Text
```
Brian from the UK.
```

#### Amazon Alexa SSML
```xml
<speak>
    <voice name="Brian"><lang xml:lang="en-GB">Brian from the UK.</lang></voice>
</speak>
```

#### Google Assistant SSML
```xml
<speak>
Brian from the UK.
</speak>
```