---
layout: page
title: SuggestFeature - Describe - Symbol to Decorators
permalink: /listiary/articles/n6vnfi356q/
exclude: true
---
<br>
```
Article type: Feature Suggestion
Article name: SuggestFeature - Describe - Symbol to Decorators
Affected Software/module: Describe Language
Author:	Framez
```
<br><br>

## Description:
Imagine a scenario - we might have some checklist - markdown style, in Describe:

```
[] 2% milk,
[] vegetable bread,
[] butter,
[] fish fillet,
```

Then, we want to be able to check or cross, as we shop, in our example:

```
[.] 2% milk,
[] vegetable bread,
[.] butter,
[x] fish fillet,
```

And, we want somehow this to work as if we have written:

```
2% milk {color|grey},
vegetable bread,
butter {color|grey},
fish fillet {color|red}{striked},
```

This can easily be achieved with few replace directives, but we need to implement 
`Front Decorators` first.

<br><br>
### Links
[Back](/listiary/articles/)<br>