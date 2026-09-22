---
layout: page
title: Bug - Describe Compiler - Tag escape
permalink: /listiary/articles/cbwnr18qn5/
exclude: true
---
<br>
```
Article type: Bug
Article name: Bug - Describe Compiler - Tag escape
Affected Software/module: Describe Compiler
Author:	Framez
```
<br><br>

### Description:
There appears to be a bug in escaping tilde - `\~`
<br><br>
```
list ->
    // cd \~ - move to home,	//that is ok
	cd \~ - move to home,		//that breaks compilation
	lorem,
	ipsum;
```

<br><br>
### Links
[Back](/listiary/articles/)<br>