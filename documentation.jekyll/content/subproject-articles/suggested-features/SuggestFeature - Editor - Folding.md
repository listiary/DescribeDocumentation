---
layout: page
title: SuggestFeature - Editor - Folding
permalink: /listiary/articles/hz6mj5sm08/
exclude: true
---
<br>
```
Article type: Feature Suggestion
Article name: SuggestFeature - Editor - Folding
Affected Software/module: Listiary Editor Module
Author:	Framez
```
<br><br>

## Description:
Editing large Describe files can be cumbersome, like editing any big code file.
This is why code editors use code folding. 
And we should do this in the Listiary editor as well. 
Here are few specific ways this might work:
<br><br>

### 1. Foldable lists
Every list - nested or standalone can be folded with an arrow in the field on the left.
<br><br>

### 2. Foldable regions
We might have special tags in comments that define folding regions.
Just like `#REGION` and `#ENDREGION` in C#.
Could be `///region` and `///endregion` - note the 3 slashes
<br><br>

### 3. Fold nowhere
Since Describe is a markup that can be prone to huge monolithic blocks of identical data,
we can add a mechanism to manually select what to fold - where to start, where to end the fold.
Again, needs to be some UI control in the left bar with the code numbers.
Of course, this data needs to be stored somewhere, probably in a cookie.

<br><br>
### Links
[Back](/listiary/articles/)<br>