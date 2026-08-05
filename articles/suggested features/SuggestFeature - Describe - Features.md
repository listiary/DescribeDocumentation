Article type: 						`Feature Suggestion`<br>
Article name:						`SuggestFeature - Describe - Features`<br>
Affected Software/module:			`Describe Compiler`<br>
Author:								`Framez`<br>
<br>

### Description:
At the moment, we have directives that allow us to choose a Describe language version
to compile against, and by choosing an earlier version, we can avoid using a feature, like tagging or decorators.

In the future, this will be implemented more gracefully, and we will have directives about the features we want 
to include or exclude.

A third and most advance implementation will be to use different parsing per list,
but that will needlessly complicate the compilation process, I would imagine, 
requiring multiple passes, and is probably not worth perusing.

### Original message:
```
Lists that get parsed without tags
Basic lists - tagging something like {basic} or {liner}
so that we can use different syntax inside those lists
we can freely use angle brackets - <> or not use commas
```