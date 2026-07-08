Article type: 						`Describe Edit`<br>
Article name:						`DescribeEdit - Edit Enlist Journal`<br>
Author:								`Framez`<br>
<br>

## Description:
This is used in lists that grow with time, like journals, data trackers, etc.
In those lists, we have a working sleeve of data, but we don't want to see an
enormously long list we will get lost into - instead, as the list grows, oldest sections
become nested lists, often named with a date, and later can be outfiled as well.
<br><br>
Such lists usially grow from top to bottom (links to archive lists accumulate at the top),
or from the bottom to the top - the newest entry is the topmost one - in which case, 
links to archive lists accumulate at the bottom.



## Before:
We have a long list.
```
directives ->
	namespace <aaa.bbb.ccc>;

Parent List <.rnode> ->

    may {comment},
	aaaa,
	bbbb,
	cccc,
	dddd,
	
	jun {nlcomment},
	eeee,
	ffff;
```



## After:
We have enlisted a chunk of the list.
```
directives ->
	namespace <aaa.bbb.ccc>;

Parent List <.rnode> ->

    may <.05> ->
		aaaa,
		bbbb,
		cccc,
		dddd;

	jun {nlcomment},
	eeee,
	ffff;
```


## Related actions:
```
Open parent list for editing
do edits, save
Ctrl+F5 on parent list article
```