Article type: 						`Feature Suggestion`<br>
Article name:						`SuggestFeature - Describe - Cumulative Directives`<br>
Affected Software/module:			`Describe Language`<br>
Author:								`Framez`<br>
<br>

## Description:
First of all, we have a directive that tells the compiler which language version to use - `language-version <1.0>`.
Then, in the future - probably in the next version of Describe we will substitute that for the ability to choose
features to turn on or off. For example:

```
using <comments>,
using <links>,
using <decorators>,
```

So then, we should have directives that do what few other directives do, in one line.
The above example can, for example be replaced with 1 single line:

```
using <basics>,
```

### Further
This is also very powerful, if there is a mechanism for the user to define his own cumulative directives,
along with templates for lists.