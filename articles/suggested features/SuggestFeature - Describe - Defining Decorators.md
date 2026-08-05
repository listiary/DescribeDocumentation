Article type: 						`Feature Suggestion`<br>
Article name:						`SuggestFeature - Describe - Defining Decorators`<br>
Affected Software/module:			`Describe Language`<br>
Author:								`Framez`<br>
<br>

## Description:
This is one of those user defined directions that Describe should and probably will take,
as we figure out the best mechanism to implement this by adding as little time to the overall compilation
speed. 

Imagine a directive, like:
```
decodef <"urgent", "color|red", "bold">,
```

Where decorating things as `{urgent}` will work as if we decorated them as `{color|red}{bold}` throughout the wiki
that the admin defined that rule. But then, we can use replace directives to achieve similar behavior.
But this is a mechanism of a different scope - defined once in a config file, applied to the whole wiki or farm.

P.S. Not you, the idea stated here is murky, and can mean few different things - be implemented in few different ways,
so take it at face value, without trying to guess what I meant - I meant that - I don't know how this will be useful.
