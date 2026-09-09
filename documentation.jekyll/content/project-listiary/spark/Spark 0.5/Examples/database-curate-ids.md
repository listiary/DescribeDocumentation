---
layout: page
title: database-curate-ids
permalink: /listiary/wiki/spark/v05/database-curate-ids/
exclude: true
---
<br>
Generate the id metadata for all the files.
<br>
This command is used to recreate the id metadata in the database.
<br><br>



### Command Syntax

`database-curate-ids [PRESENTATION_FLAGS]`<br>
`PRESENTATION_FLAGS` - common presentation flags for the SparkCli.<br>
For more info on presentation flags, check the [Presentation flags manual](/listiary/wiki/spark/v05/pflags/).
<br><br>



### Examples
`php spark.php database-curate-ids`<br>
Recreate the id-specific metadata in the database.
<br><br>
`php spark.php database-curate-ids theme=DEFAULT`<br>
Recreate the id-specific metadata in the database, with presentation flags
<br><br>
`php spark.php database-curate-ids -hb theme=DEFAULT`<br>
Recreate the id-specific metadata in the database, with presentation flags
<br><br>
`php spark.php database-curate-ids -auto -hb theme=DEFAULT`<br>
Recreate the id-specific metadata in the database, with presentation flags
<br><br>


### Links
[Back](/listiary/wiki/spark/v05/)