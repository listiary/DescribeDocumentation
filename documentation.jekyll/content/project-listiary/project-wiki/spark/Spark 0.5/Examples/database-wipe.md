---
layout: page
title: database-wipe
permalink: /listiary/wiki/spark/v05/database-wipe/
exclude: true
---
<br>
Wipe a database empty. The nuclear option.
<br>
This command is used to uninstall a Listiary wiki, or to prepare a database for a wiki installation.
<br>
This command is dangerous.
<br><br>


### Command Syntax

`database-wipe [PRESENTATION_FLAGS]`<br>
`PRESENTATION_FLAGS` - common presentation flags for the SparkCli.<br>
For more info on presentation flags, check the [Presentation flags manual](/listiary/wiki/spark/v05/pflags/).
<br><br>



### Examples
`php spark.php database-wipe`<br>
Wipe a database for wiki installation.
<br><br>
`php spark.php database-wipe theme=DEFAULT`<br>
Wipe a database for wiki installation with presentation flags
<br><br>
`php spark.php database-wipe -hb theme=DEFAULT`<br>
Wipe a database for wiki installation with presentation flags
<br><br>
`php spark.php database-wipe -auto -hb theme=DEFAULT`<br>
Wipe a database for wiki installation with presentation flags
<br><br>


### Links
[Back](/listiary/wiki/spark/v05/)