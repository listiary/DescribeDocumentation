---
layout: page
title: SuggestFeature - Describe - Nl Decorators
permalink: /listiary/articles/oriakpjtou/
exclude: true
---
<br>
```
Article type: Feature Suggestion
Article name: SuggestFeature - Describe - Nl Decorators
Affected Software/module: Describe Language
Author:	Framez
```
<br><br>

## Description:

The NL decorator `{nl}` is needed to produce a new line before an entry - producing
an empty entry before it. We can achieve that with the EMPTY decorator - writing something like `gap {empty},`,
as our current grammar does not allow for empty entries without text - so we add the text 'gap', and the entry
gets translated to an empty one, none the less.
<br><br>
We have implemented the NLCOMMENT decorator, that does something similar for a comment.
For example, here is a comment, that will have an empty entry before it - `some comment {nlcomment},`.
<br><br>
What I propose is that, it would be only logical to have the same style of new line-inducing decorator
for regular entries.
<br><br>
We can also introduce decorators like `{nl2}` and `{nl3}`, for 2 or 3 new lines.

<br><br>
### Links
[Back](/listiary/articles/)<br>