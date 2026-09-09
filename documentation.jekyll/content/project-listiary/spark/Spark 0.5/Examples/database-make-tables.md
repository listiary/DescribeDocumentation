---
layout: page
title: database-make-tables
permalink: /listiary/wiki/spark/v05/database-make-tables/
exclude: true
---
<br>
Make the tables in an empty database, installing a wiki instance.
<br>
This command is used to create all the tables, in a wiki installation.
<br><br>



### Command Syntax

`database-make-tables [PRESENTATION_FLAGS]`<br>
`PRESENTATION_FLAGS` - common presentation flags for the SparkCli.<br>
For more info on presentation flags, check the [Presentation flags manual](/listiary/wiki/spark/v05/pflags/).
<br><br>



### Examples
`php spark.php database-make-tables`<br>
Prepare a database for wiki installation.
<br><br>
`php spark.php database-make-tables theme=DEFAULT`<br>
Prepare a database for wiki installation with presentation flags
<br><br>
`php spark.php database-make-tables -hb theme=DEFAULT`<br>
Prepare a database for wiki installation with presentation flags
<br><br>
`php spark.php database-make-tables -auto -hb theme=DEFAULT`<br>
Prepare a database for wiki installation with presentation flags
<br><br>


### Links
[Back](/listiary/wiki/spark/v05/)