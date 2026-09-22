---
layout: page
title: config-show
permalink: /listiary/wiki/spark/v05/config-show/
exclude: true
---
<br>
Show the constants inside the selected config.<br>
Output the values in that file to the console.
<br><br>
If no `CONFIG_NAME` parameter is provided, the config that will be shown will be the default one - 
the one named `config.php`.


### Command Syntax
`config-show [CONFIG_NAME] [PRESENTATION_FLAGS]`<br>
`CONFIG_NAME` - The name of the config in the `_configs` folder, to be viewed.<br>
`PRESENTATION_FLAGS` - common presentation flags for the SparkCli.<br>
For more info on presentation flags, check the [Presentation flags manual](/listiary/wiki/spark/v05/pflags/).
<br><br>



### Examples
`php spark.php config-show`<br>
show the default config.
<br><br>
`php spark.php config-show theme=DEFAULT`<br>
show the default config, with presentation flags
<br><br>
`php spark.php config-show -hb theme=DEFAULT`<br>
show the default config, with presentation flags
<br><br>
`php spark.php config-show -auto -hb theme=DEFAULT`<br>
show the default config, with presentation flags
<br><br>
`php spark.php config-show "configA.php"`<br>
show a config.
<br><br>
`php spark.php config-show "configA.php" theme=DEFAULT`<br>
show a config, with presentation flags
<br><br>
`php spark.php config-show "configA.php" -hb theme=DEFAULT`<br>
show a config, with presentation flags
<br><br>
`php spark.php config-show "configA.php" -auto -hb theme=DEFAULT`<br>
show a config, with presentation flags
<br><br>


### Links
[Back](/listiary/wiki/spark/v05/)