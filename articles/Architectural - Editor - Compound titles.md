Article type: 						`Architectural`<br>
Article name:						`Architectural - Editor - Compound titles`<br>
Affected Software/module:			`Editor Module`<br>
Author:								`Framez`<br>

## Description:
We should definitely switch from CodeMirror code editing library/component
to Monaco, as CodeMirror is terrible, especially on mobile.
<br>
Then we can implement some syntax highlighting.
In the viewer that can be easy - we need the parsing action execute once for the highlighting.
<br>
But for a real-time highlighting - we will need to re-implement the Describe compiler in JS.
Otherwise, we will hammer our C# AWS Lambda setup too much.
Which is extremely doable, since we are using ANTLR for the Describe compiler - and ANTLR4 supports 
JavaScript, PHP, and few other languages. But it will be a bit of a hassle.
<br>

```
Realtime syntax highlighting using Monaco or CodeMirror
```