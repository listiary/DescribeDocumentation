Article type: 						`Bug`<br>
Article name:						`Bug - Describe Compiler - Tag escape`<br>
Affected Software/module:			`Describe Compiler`<br>
Author:								`Framez`<br>
<br>

## Description:
There appears to be a bug in escaping tilde - `\~`
<br><br>
```
list ->
    // cd \~ - move to home,	//that is ok
	cd \~ - move to home,		//that breaks compilation
	lorem,
	ipsum;
```