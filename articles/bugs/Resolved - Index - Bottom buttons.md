Article type: Resolved<br>
Article name: Resolved - Index - Bottom buttons<br>
Affected Software/module: Listiary Index Module<br>
Author: Framez<br>

The issue here was that, when we make the bottom circular buttons visible at all times, we get situations where they are not needed and look bad.
<br>
So our decision was to require a content on the page of significant length before the controls are allowed to be shown.
<br>
However, in the future, we'll need to revisit the way we are doing that calculation, and generally figure out if there will be a footer, and how will it be designed to look and behave.
<br>
The original description was this :
```
make lengthier lists needed to add the bottom controls - otherwise they are half-visible
```