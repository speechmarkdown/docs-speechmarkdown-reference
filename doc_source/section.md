# section

A section tag marks the beginning of a section. The section continues until the next section tag is found or the end of the content is reached.

The format of a section is: `#[key:"value";...]`

Sections can include the following markdown:
+ [lang](lang.md)
+ [voice](voice.md)


```
My voice and language is based on the device.

#[voice:"Kendra";lang:"en-US"]
Now I am speaking as Kendra from the US with a US accent.

#[voice:"Brian";lang:"en-US"]
Switching to Brian from the UK with a US accent.

#[voice:"device"]
Now back to the device setting.
```
