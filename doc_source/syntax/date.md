# date

Speak the text as a date.

The date can use various separators:

- slash - 10/11/12
- dash - 10-11-12
- dot - 10.11.12

Some SSML formatters require the year to be 4 digits. Some might auto-expand 2-digit years to 4 digits.

```text
The date is (10-11-12)[date:"mdy"].     // October 11th, 2012
The date is (10-11-12)[date:"dmy"].     // November 10th, 2012
The date is (10-11-12)[date:"ymd"].     // Nov 12th, 2010
The date is (10-11-12)[date:"ydm"].     // December 11th, 2010
The date is (10-11)[date:"md"].         // October 11th
The date is (10-11)[date:"dm"].         // November 10th
The date is (10-11)[date:"ym"].         // November 2010
The date is (10-11)[date:"my"].         // October 2011
The date is (10)[date:"y"].             // 2010
The date is (10)[date:"m"].             // October
The date is (10)[date:"d"].             // 10th
```
The following format values are accepted:

- mdy
- dmy
- ymd
- ydm (not universal support)
- md
- dm
- ym
- my
- y
- m
- d

---

### Speech Markdown
#### Short format
```text
n/a
```

#### Standard format
```text
The date is (10-19-2016)[date:"mdy"].
```

### Formatters
#### Plain Text
```text
The date is 10-19-2016.
```

#### Amazon Alexa SSML
Alexa SSML does not support `format="ydm"`. Two-digit years are automatically expanded to 4-digit years. (ex: from 10 to 2010)

```xml
<speak>
    The date is <say-as interpret-as="date" format="mdy">10-11-12</say-as>.
    The date is <say-as interpret-as="date" format="dmy">10-11-12</say-as>.
    The date is <say-as interpret-as="date" format="ymd">10-11-12</say-as>.
    The date is 10-11-12.   // no support for format="ydm"
    The date is <say-as interpret-as="date" format="md">10-11</say-as>.
    The date is <say-as interpret-as="date" format="dm">10-11</say-as>.
    The date is <say-as interpret-as="date" format="ym">10-11</say-as>.
    The date is <say-as interpret-as="date" format="my">10-11</say-as>.
    The date is <say-as interpret-as="date" format="y">10</say-as>.
    The date is <say-as interpret-as="date" format="m">10</say-as>.
    The date is <say-as interpret-as="date" format="d">10</say-as>.
</speak>
```

#### Google Assistant SSML
```xml
<speak>
    The date is <say-as interpret-as="date" format="mdy">10-11-12</say-as>.
    The date is <say-as interpret-as="date" format="dmy">10-11-12</say-as>.
    The date is <say-as interpret-as="date" format="ymd">10-11-12</say-as>.
    The date is <say-as interpret-as="date" format="ydm">10-11-12</say-as>.
    The date is <say-as interpret-as="date" format="md">10-11</say-as>.
    The date is <say-as interpret-as="date" format="dm">10-11</say-as>.
    The date is <say-as interpret-as="date" format="ym">10-11</say-as>.
    The date is <say-as interpret-as="date" format="my">10-11</say-as>.
    The date is <say-as interpret-as="date" format="y">10</say-as>.
    The date is <say-as interpret-as="date" format="m">10</say-as>.
    The date is <say-as interpret-as="date" format="d">10</say-as>.
</speak>
```
