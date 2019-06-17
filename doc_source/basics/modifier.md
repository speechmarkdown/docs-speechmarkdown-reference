# Modifiers

A modifier is Speech Markdown that changes the way a specific word or phrase is spoken.

The typical format of a modifier is: `(text)[key:"value";...]`

Not all modifiers have a value. Multiple modifiers can be applied to the same text.

```text
This is some (content with modifiers)[volume:"loud";rate:"slow"]

A (moderate)[emphasis] level

The word is spelled: (hello)[spell-out]

The date is: (10/11/12)[date:"mdy"]
```

Modifiers can include the following markdown:

+ [address](../syntax/address)
+ [audio](../syntax/audio)
+ [break](../syntax/break)
+ [cardinal](../syntax/cardinal)
+ [characters](../syntax/characters)
+ [date](../syntax/date)
+ [digits](../syntax/digits)
+ [emphasis](../syntax/emphasis)
+ [expletive / bleep](../syntax/expletive)
+ [fraction](../syntax/fraction)
+ [interjection](../syntax/interjection)
+ [ipa](../syntax/ipa)
+ [lang](../syntax/lang)
+ [number](../syntax/number)
+ [ordinal](../syntax/ordinal)
+ [phone / telephone](../syntax/phone)
+ [pitch](../syntax/pitch)
+ [rate](../syntax/rate)
+ [spell-out](../syntax/spell-out)
+ [sub](../syntax/sub)
+ [time](../syntax/time)
+ [unit](../syntax/unit)
+ [verbatim](../syntax/verbatim)
+ [voice](../syntax/voice)
+ [volume / vol](../syntax/volume)
+ [whisper](../syntax/whisper)