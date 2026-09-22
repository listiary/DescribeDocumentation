---
layout: page
title: DescribeEdit - Add List Outfile
permalink: /listiary/articles/sbr88h14eq/
exclude: true
---
<br>
```
Article type: Describe Edit
Article name: DescribeEdit - Add List Outfile
Author: Framez
```
<br>

## Description:
We add the list's head just as another item in the parent list.<br>
We create a new file with the proper name for the new list.
<br><br>


## Before:
We have a parent list.<br>
file name - `aaa.bbb.ccc`
```
directives ->
	namespace <aaa.bbb.ccc>;

Parent List <.rnode> ->
	lorem,
	ipsum;
```
<br><br>

## After:
We have 2 files<br>
file A - parent - `aaa.bbb.ccc`
```
directives ->
	namespace <aaa.bbb.ccc>;

Parent List <.rnode> ->
	lorem,
	dolor <.dol>,
	ipsum;
```

file B - outfile - `aaa.bbb.ccc.dol`
```
directives ->
	namespace <aaa.bbb.ccc>;

dolor <.dol> ->
	aaaaa,
	bbbbb;
```
<br><br>

## Related actions:
```
Open parent list for editing
php spark.php action-create-stub "TEXT" "NAMESPACE.NAME"
open "https://development.listiary.org/m.editor/m.editor.php?domain=public&itemid=0&article=NAMESPACE.NAME"
do edits on both files
save both files, I think the new one first
Ctrl+F5 on parent list article
```
<br><br>

<br><br>
### Links
[Back](/listiary/articles/)<br>