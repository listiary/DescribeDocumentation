---
layout: page
title: database-curate
permalink: /listiary/wiki/spark/v05/database-curate/
exclude: true
---
<br>
Generate the full metadata for all the files.
<br>
This command is used to recreate the metadata in the database.
<br><br>



### Command Syntax

`database-curate [PRESENTATION_FLAGS]`<br>
`PRESENTATION_FLAGS` - common presentation flags for the SparkCli.<br>
For more info on presentation flags, check the [Presentation flags manual](/listiary/wiki/spark/v05/pflags/).
<br><br>



### Examples
`php spark.php database-curate`<br>
Recreate the metadata in the database.
<br><br>
`php spark.php database-curate theme=DEFAULT`<br>
Recreate the metadata in the database, with presentation flags
<br><br>
`php spark.php database-curate -hb theme=DEFAULT`<br>
Recreate the metadata in the database, with presentation flags
<br><br>
`php spark.php database-curate -auto -hb theme=DEFAULT`<br>
Recreate the metadata in the database, with presentation flags
<br><br>


### Links
[Back](/listiary/wiki/spark/v05/)