Article type: 						`Describe Edit`<br>
Article name:						`DescribeEdit - Edit Downmove Entry`<br>
Author:								`Framez`<br>
<br>

## Description:
This is used in lists that grow with time, like task lists, shopping lists, etc.
In those list, we might have an entry that we want to move around to the bottom.<br>

Imagine this scenario - there is a shopping list, and it calls for buying salt.
But the user never got to do it - so we want to cut the entry from few days ago, and paste it for today,
so that it is in the newest section of the shopping list.<br>

This is downmoving - cutting something older and pushing it as new.



## Before:
We have a long list.
```
directives ->
	namespace <aaa.bbb.ccc>;

Parent List <.rnode> ->

    Thu {comment},
	grab breakfast {color|grey},
	buy coffee {color|grey},
	buy salt,
	buy eggs {color|grey},
	
	Fri {nlcomment},
	grab breakfast;
```



## After:
We have downmoved the "buy salt" entry.
```
directives ->
	namespace <aaa.bbb.ccc>;

Parent List <.rnode> ->

    Thu {comment},
	grab breakfast {color|grey},
	buy coffee {color|grey},
	buy eggs {color|grey},
	
	Fri {nlcomment},
	grab breakfast,
	buy salt;
```


## Related actions:
```
Open parent list for editing
do edits, save
Ctrl+F5 on parent list article
```