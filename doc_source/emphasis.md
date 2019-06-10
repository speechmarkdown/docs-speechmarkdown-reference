# emphasis

Add or remove emphasis from a word or phrase.

```
A ++strong++ level
A +moderate+ level
A ~none~ level
A -reduced- level


A (strong)[emphasis:"strong"] level

A (moderate)[emphasis] level
A (moderate)[emphasis:"moderate"] level

A (none)[emphasis:"none"] level

A (reduced)[emphasis:"reduced"] level
```

## level

Set break length in seconds or milliseconds:
- strong
- moderate (default)
- none
- reduced


### Speech Markdown
#### Short format
```
A ++strong++ level
A +moderate+ level
A ~none~ level
A -reduced- level
```

#### Standard format
```
A (strong)[emphasis:"strong"] level

A (moderate)[emphasis] level
A (moderate)[emphasis:"moderate"] level

A (none)[emphasis:"none"] level

A (reduced)[emphasis:"reduced"] level
```

### Formatters
#### Plain Text
```
A strong level
A moderate level
A none level
A reduced level
```

#### Amazon Alexa SSML
```
A <emphasis level="strong">strong</emphasis> level

A <emphasis level="moderate">moderate</emphasis> level
A <emphasis>moderate</emphasis> level

A <emphasis level="none">none</emphasis> level

A <emphasis level="reduced">reduced</emphasis> level
```

#### Google Assistant SSML
```
A <emphasis level="strong">strong</emphasis> level

A <emphasis level="moderate">moderate</emphasis> level
A <emphasis>moderate</emphasis> level

A <emphasis level="none">none</emphasis> level

A <emphasis level="reduced">reduced</emphasis> level
```