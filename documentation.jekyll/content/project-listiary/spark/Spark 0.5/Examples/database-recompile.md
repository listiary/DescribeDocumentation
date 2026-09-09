---
layout: page
title: database-recompile
permalink: /listiary/wiki/spark/v05/database-recompile/
exclude: true
---
<br>
Recompile all the files in the database.
<br>
Use this command to recompile all the raw Describe source files in the database to create/recreate the JSON files in the database.
<br>
This command is useful when troubleshooting some bug, to recover from a bad state.
<br><br>



### Command Syntax

`database-recompile [PRESENTATION_FLAGS]`<br>
`PRESENTATION_FLAGS` - common presentation flags for the SparkCli.<br>
For more info on presentation flags, check the [Presentation flags manual](/listiary/wiki/spark/v05/pflags/).
<br><br>



### Examples
`php spark.php database-recompile`<br>
Recompile a database.
<br><br>
`php spark.php database-recompile theme=DEFAULT`<br>
Recompile a database, with presentation flags
<br><br>
`php spark.php database-recompile -hb theme=DEFAULT`<br>
Recompile a database, with presentation flags
<br><br>
`php spark.php database-recompile -auto -hb theme=DEFAULT`<br>
Recompile a database, with presentation flags
<br><br>


### Links
[Back](/listiary/wiki/spark/v05/)