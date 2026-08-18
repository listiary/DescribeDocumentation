---
layout: page
title: DescribeEdit - Add List Inline
permalink: /listiary/articles/dze5ciiyzq/
exclude: true
---
<br>
```
Article type: Describe Edit
Article name: DescribeEdit - Add List Inline
Author: Framez
```
<br>

## Description:
In this edit, we will add a list directly inline in another list.
This will be very simple - no new files, no need to decide on a namespace, etc.
It is also the ugliest, and discouraged for public articles for long term.
<br><br>
We just add the list's head just as another item in the parent list, add the production arrow,
and write our list. We use a proper indentation - in this case one level deeper, for readability.
<br><br>
We need to make sure to use a proper tag format (it will be a navigable list, so we need a public tag),
make sure to properly close any trailing nested lists in our inline lists, if it is not the last element,
and make sure to properly close any trailing nested lists in the parent list's previous element, if our inline list is not the first element.
<br><br>

## Before:
We have a parent list.
```
directives ->
	namespace <aaa.bbb.ccc>;

Parent List <.rnode> ->
	lorem,
	ipsum;
```
<br><br>

## After:
We have the inserted inline list, in this case at some middle position - 
that is, not first, not last.
```
directives ->
	namespace <aaa.bbb.ccc>;

Parent List <.rnode> ->

	lorem,
	dolor <.dol> ->
		sit,
		amet;
	ipsum,
	dolor <.dol>;
```

B - A more elaborate example
```
directives ->
	namespace <aaa.bbb.ccc>;

Parent List <.rnode> ->

	lorem,
	dolor <.dol> ->
		sit,
		amet <.ame> ->
			xxx,
			yyy
		;
	;	
	ipsum,
	dolor <.dol>;
```
<br><br>

## Related actions:
```
Open parent list for editing
do edits, save
Ctrl+F5 on parent list article
```

<br><br>
### Links
[Back](/listiary/articles/)<br>