# Formatters

If all voice platforms natively and consistently supported Speech Markdown, there would be no need for formatters. As we stand today, Speech Synthesis Markup Language (SSML) is all that is supported. Because each of the platforms have different levels of support for SSML (and in some cases introduced their own extensions) there are multiple flavors of SSML. For example, the SSML used by Amazon Alexa is mostly the same but different from that of Google Assistant. (For a quick comparison, see [SSML Guru](http://ssml.guru))

The solution is to parse Speech Markdown into a intermediate format and then use formatters to convent it into plain text (remove any markdown formatting) or a platform-specific flavor of SSML.

For developers, that intermediate format is an Abstract Syntax Tree (AST).