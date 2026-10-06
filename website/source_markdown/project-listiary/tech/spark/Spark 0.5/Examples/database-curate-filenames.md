---
layout: page
title: database-curate-filenames
permalink: /listiary/wiki/spark/v05/database-curate-filenames/
exclude: true
---
<br>
Generate the filename-related metadata for all the files.
<br>
This command is used to recreate the filename-related metadata in the database.
<br><br>



### Command Syntax

`database-curate-filenames [PRESENTATION_FLAGS]`<br>
`PRESENTATION_FLAGS` - common presentation flags for the SparkCli.<br>
For more info on presentation flags, check the [Presentation flags manual](/listiary/wiki/spark/v05/pflags/).
<br><br>



### Examples
`php spark.php database-curate-filenames`<br>
Recreate the filename-specific metadata in the database.
<br><br>
`php spark.php database-curate-filenames theme=DEFAULT`<br>
Recreate the filename-specific metadata in the database, with presentation flags
<br><br>
`php spark.php database-curate-filenames -hb theme=DEFAULT`<br>
Recreate the filename-specific metadata in the database, with presentation flags
<br><br>
`php spark.php database-curate-filenames -auto -hb theme=DEFAULT`<br>
Recreate the filename-specific metadata in the database, with presentation flags
<br><br>


### Links
[Back](/listiary/wiki/spark/v05/)