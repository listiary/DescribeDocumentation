---
layout: page
title: Bug - Describe Compiler - Tilde escape
permalink: /listiary/articles/aue8tbh215/
exclude: true
---
<br>
```
Article type: Bug
Article name: Bug - Describe Compiler - Tilde escape
Affected Software/module: Describe Compiler
Author:	Framez
```
<br><br>

### Description:
Escaping left angle bracket produces a right angle bracket in the final text
<br><br>
```
      adb shell pm uninstall --user 0 \<PACKAGE_NAME\> {color|blue}, 
      uninstall a package {comment},
      gap {empty},
```

This produces a text `adb shell pm uninstall --user 0 >PACKAGE_NAME>`


<br><br>
### Links
[Back](/listiary/articles/)<br>