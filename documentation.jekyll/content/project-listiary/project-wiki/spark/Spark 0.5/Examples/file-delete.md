---
layout: page
title: file-delete
permalink: /listiary/wiki/spark/v05/file-delete/
exclude: true
---
<br>
Delete a single Describe file in the database.
<br>
The user runs a command like `files-list` to list the raw files in the database,
then runs `file-delete` to delete a single file.
<br>
This command is useful when there is some kind of a bug, and we want to delete
a file, where something went wrong and we are manually fixing it, before recompiling the database.
<br><br>


### Command Syntax
`file-delete FILE_NAME [PRESENTATION_FLAGS]`<br>
`FILE_NAME` - The name of the file in the database.<br>
`PRESENTATION_FLAGS` - common presentation flags for the SparkCli.<br>
For more info on presentation flags, check the [Presentation flags manual](/listiary/wiki/spark/v05/pflags/).
<br><br>



### Examples
`php spark.php file-delete "root.name"`<br>
Delete a file
<br><br>
`php spark.php file-delete "root.name" theme=DEFAULT`<br>
Delete a file with presentation flags
<br><br>
`php spark.php file-delete "root.name" -hb theme=DEFAULT`<br>
Delete a file with presentation flags
<br><br>
`php spark.php file-delete "root.name" -auto -hb theme=DEFAULT`<br>
Delete a file with presentation flags
<br><br>


### Links
[Back](/listiary/wiki/spark/v05/)