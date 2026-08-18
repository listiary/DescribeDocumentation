Pluginlets - plugins per instance

The Listiary index module supports plugins, and comes with some readily available.
Admins can choose whether to enable or disable them, per wiki instance.

Admins can also develop their own plugins. The requirement is that those are written in vanilla JS only, and have no dependencies. 

Or rather, it is a guideline some admins might choose to ignore in the future. But I see the pluginlets as small, 1 file apps written in plain JS, that interact with the data in the loaded article to figure out if they should run in that page, and if so, they modify the content in some way, or add a control on top of the list, for example.