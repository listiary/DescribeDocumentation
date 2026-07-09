Article type: 						`Describe Edit`<br>
Article name:						`DescribeEdit - Edit Downcopy Entry`<br>
Author:								`Framez`<br>
<br>

## Description:
This is used in lists that grow with time, like task lists, shopping lists, etc.
In those list, we might have an entry that we want to copy to the bottom.<br>

Imagine this scenario - there is a shopping list, and it called for buying salt a month ago.
And now, it is time to buy salt again, so we want to copy that entry for from few weeks ago, and paste it for today,
so that it is in the newest section of the shopping list, while maybe changing few attributes as well.<br>

Or maybe the user forgot to buy salt yesterday - the entry was marked in red, and now, same thing -
we want to copy that entry, and remove the color decorator.<br>

This is downcopying - copying something older and pushing it as new.



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
We have downcopied the "buy salt" entry.
```
directives ->
	namespace <aaa.bbb.ccc>;

Parent List <.rnode> ->

    Thu {comment},
	grab breakfast {color|grey},
	buy coffee {color|grey},
	buy salt {color|red},
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