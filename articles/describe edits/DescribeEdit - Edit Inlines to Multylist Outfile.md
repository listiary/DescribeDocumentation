Article type: 						`Describe Edit`<br>
Article name:						`DescribeEdit - Edit Inlines to Multylist Outfile`<br>
Author:								`Framez`<br>
<br>

## Description:
We have 2 or more lists, contained inline in another list, that we want to export to another file.<br>
We will need to create the new article, from those lists, and remove the body of the lists from the original file.
Then, we re-Curate the database, or just the affected entries.

## Before:
We have a parent list, containing an inline list.<br>
File probably named - `aaa.bbb.ccc`
```
directives ->
	namespace <aaa.bbb.ccc>;

Parent List <.rnode> ->

	lorem,
	ipsum,
	
	dolor <.dol> ->
		sit,
		amet;
		
	elit <.el> ->
		sed,
		tempor;
```

## After:
A - the parent list has the exportees bodies trimmed, and the exportees reduced to entries.<br>
File still probably named - `aaa.bbb.ccc`
```
directives ->
	namespace <aaa.bbb.ccc>;

Parent List <.rnode> ->

	lorem,
	ipsum,
	dolor <.dol>,
	elit <.el>;
```

B - the exportees are declared in a new file, with 2 root lists<br>
New file probably named - `aaa.bbb.ccc.dol`
```
directives ->
	namespace <aaa.bbb.ccc>;

dolor <.dol> ->
	sit,
	amet;
	
elit <.el> ->
	sed,
	tempor;
```

## Related actions:
```
php spark.php action-create-stub "TEXT" "full.namespace.name"
open "https://development.listiary.org/m.editor/m.editor.php?domain=public&itemid=0&article=full.namespace.name"
cut body from parent list, paste to child file.
save both lists and close the child file editor.
php spark.php database-curate
Ctrl+F5 on parent list
```