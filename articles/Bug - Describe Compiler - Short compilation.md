Article type: 						`Bug`<br>
Article name:						`Bug - Describe Compiler - Short compilation`<br>
Affected Software/module:			`Describe Compiler`<br>
Author:								`Framez`<br>
<br>

## Description:
having two lists, where one includes a reference to the other, 
makes the second list compile just like a leaf.
<br><br>
This is not supposed to happen, and we need to investigate it
<br><br><br>


## Example

List 1, in a Describe source file:
```
sddssd ->

   aaa,
   bbb <.bb>;
```
<br>

List 2 - in a separate file:

```
bbb <.bb> ->

   lorem,
   ipsum;
```