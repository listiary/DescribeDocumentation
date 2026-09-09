---
layout: page
title: action-delete-article
permalink: /listiary/wiki/spark/v05/action-delete-article/
exclude: true
---
<br>
Delete an article and all its files.
<br><br>



### Command Syntax

`action-delete-article "FILENAME" [PRESENTATION_FLAGS]`<br>
`FILE_NAME` - The name of the article in the database to be deleted<br>
`PRESENTATION_FLAGS` - common presentation flags for the SparkCli.<br>
For more info on presentation flags, check the [Presentation flags manual](/listiary/wiki/spark/v05/pflags/).
<br><br>



### Examples
`php spark.php action-delete-article "file.name"`<br>
Recreate the metadata in the database.
<br><br>
`php spark.php action-delete-article "file.name" theme=DEFAULT`<br>
Recreate the metadata in the database, with presentation flags
<br><br>
`php spark.php action-delete-article "file.name" -hb theme=DEFAULT`<br>
Recreate the metadata in the database, with presentation flags
<br><br>
`php spark.php action-delete-article "file.name" -auto -hb theme=DEFAULT`<br>
Recreate the metadata in the database, with presentation flags
<br><br>


### Links
[Back](/listiary/wiki/spark/v05/)