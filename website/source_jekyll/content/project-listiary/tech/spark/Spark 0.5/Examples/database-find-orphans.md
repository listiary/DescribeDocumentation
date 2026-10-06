---
layout: page
title: database-find-orphans
permalink: /listiary/wiki/spark/v05/database-find-orphans/
exclude: true
---
<br>
Find orphaned articles in the database
<br>
This command is used to help editing, by finding articles that are not connected to the rest.
<br><br>



### Command Syntax

`database-find-orphans [PRESENTATION_FLAGS]`<br>
`PRESENTATION_FLAGS` - common presentation flags for the SparkCli.<br>
For more info on presentation flags, check the [Presentation flags manual](/listiary/wiki/spark/v05/pflags/).
<br><br>



### Examples
`php spark.php database-find-orphans`<br>
Find all the orphan lists in the database.
<br><br>
`php spark.php database-find-orphans theme=DEFAULT`<br>
Find all the orphan lists in the database, with presentation flags
<br><br>
`php spark.php database-find-orphans -hb theme=DEFAULT`<br>
Find all the orphan lists in the database, with presentation flags
<br><br>
`php spark.php database-find-orphans -auto -hb theme=DEFAULT`<br>
Find all the orphan lists in the database, with presentation flags
<br><br>


### Links
[Back](/listiary/wiki/spark/v05/)