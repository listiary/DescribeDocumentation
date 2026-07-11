Article type: 						`Feature Suggestion`<br>
Article name:						`SuggestFeature - Index - Indexed lists`<br>
Affected Software/module:			`Listiary Index Module`<br>
Author:								`Framez`<br>
<br>

## Description:
There should be few decorators in Describe about what HTML calls 'ordered lists'
That is simply, prefixing each entry with a number, or a letter, or something.
<br><br>
For one, we might use `{numlist}` for a numbered list, and something like:<br>

`{prefix-X}` - where X is a format specifier.<br>
`{prefix-1}` - for numeric - same as `{numlist}`<br>
`{prefix-a}` - for lowercase alphabetical list<br>
`{prefix-A}` - for uppercase alphabetical list<br>
`{prefix-c}` - for uppercase alphabetical list, if we don't support case sensitive decorators<br>
`{prefix-i}` - for roman numeral prefixed list<br>
`{prefix-bullet}` - for bullet-prefixed list - `•`<br>
`{prefix-moon}` - for half-moon-prefixed list, showing legend colors for example - `◑︎`