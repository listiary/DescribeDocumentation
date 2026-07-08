Article type: 						`Describe Edit`<br>
Article name:						`DescribeEdit - Add List Local`<br>
Author:								`Framez`<br>
<br>

## Description:
Here, we add a list within the same file.
We just add the list's head just as another item in the parent list,
Add the full list with the title at the bottom of the document, or after the parent list ends
being careful to properly close any trailing nested lists of the parent,
as to prevent accidental new list inclusion in the parent's end



## Before:
We have a parent list.
```
directives ->
	namespace <aaa.bbb.ccc>;

Parent List <.rnode> ->
	lorem,
	ipsum;
```



## After:
We have the inserted inline list, in this case at some middle position - 
that is, not first, not last.
```
directives ->
	namespace <aaa.bbb.ccc>;

Parent List <.rnode> ->
	lorem,
	dolor <.dol>,
	ipsum;
	
dolor <.dol> ->
	sit,
	amet;
```


## Related actions:
```
Open parent list for editing
do edits, save
Ctrl+F5 on parent list article
```