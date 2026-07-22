---
layout: page
title: file-view
permalink: /listiary/wiki/spark/v05/file-view/
exclude: true
---
<br>
Fetch a single file from the database.
Output the contents of that file to the console.
<br><br>


### Command Syntax
`file-view FILE_NAME [PRESENTATION_FLAGS]`<br>
`FILE_NAME` - The name of the raw source file in the database to be viewed<br>
`PRESENTATION_FLAGS` - common presentation flags for the SparkCli.<br>
For more info on presentation flags, check the [Presentation flags manual](/listiary/wiki/spark/v05/pflags/).
<br><br>



### Examples
`php spark.php file-view "root.name"`<br>
view a file
<br><br>
`php spark.php file-view "root.name" theme=DEFAULT`<br>
view a file with presentation flags
<br><br>
`php spark.php file-view "root.name" -hb theme=DEFAULT`<br>
view a file with presentation flags
<br><br>
`php spark.php file-view "root.name" -auto -hb theme=DEFAULT`<br>
view a file with presentation flags
<br><br>


### Links
[Back](/listiary/wiki/spark/v05/)