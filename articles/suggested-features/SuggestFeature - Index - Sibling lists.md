Article type: 						`Feature Suggestion`<br>
Article name:						`SuggestFeature - Index - Sibling lists`<br>
Affected Software/module:			`Listiary Index Module`<br>
Author:								`Framez`<br>
<br>

## Description:
Sibling lists - those can be switched to with an icon near the top - every sibling
list has an icon. If they are defined with a list, that list's structure can be translated to those icons structure.
For our second example below, we can have icons order:

```
(2)(3)
   (4)
-------------------------------------------------------
list 1 ->

  :sibling <list2id>,
  :sibling <list3id>,

  some,
  items;

list 1 ->

  :siblings ->
    list2id, list3id,
    list4id;

  some,
  items;
-------------------------------------------------------
```