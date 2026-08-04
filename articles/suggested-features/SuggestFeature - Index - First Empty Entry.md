Article type: 						`Feature Suggestion`<br>
Article name:						`SuggestFeature - Index - First Empty Entry`<br>
Affected Software/module:			`Index Module`<br>
Author:								`Framez`<br>
<br>

## Description:

When we have an empty entry at the beginning of the list, as the first entry,
or if we have a decorator, like NLCOMMENT that facilitates that, 
this functionality should be ignored, as we don't need empty entries
at the beginning of a list (or at the end, as a matter of fact),
because they are delimiters, and this destroys the purpose.

### Original draft text:
```
using empty item at the beginning of a list
should not work, same as nlcomment be translated as comment
```