Article type: 						`Feature Suggestion`<br>
Article name:						`SuggestFeature - Editor - Highlighting`<br>
Affected Software/module:			`Listiary Editor Module`<br>
Author:								`Framez`<br>
<br>

## Description:
We need to utilize the Describe compiler to produce debug data - a syntax tree
which - the functionality is there, to do code highlighting.
<br><br>
But it will never be instant until we rewrite the Describe compiler to run in PHP,
or we will be hammering our AWS lambda every few seconds per an opened editor.
Still, we can do it at the beginning of opening an editor - and also implement it without
a UI button - something like "check syntax"