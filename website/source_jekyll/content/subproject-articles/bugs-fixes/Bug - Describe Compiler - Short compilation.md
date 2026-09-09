---
layout: page
title: Bug - Describe Compiler - Short compilation
permalink: /listiary/articles/gjid1sa3u0/
exclude: true
---
<br>
```
Article type: Bug
Article name: Bug - Describe Compiler - Short compilation
Affected Software/module: Describe Compiler
Author:	Framez
```
<br><br>

### Description:
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
<br><br>

List 2 - in a separate file:

```
bbb <.bb> ->

   lorem,
   ipsum;
```

<br><br>
### Links
[Back](/listiary/articles/)<br>