---
layout: page
title: files-list
permalink: /listiary/wiki/spark/v05/files-list/
exclude: true
---
<br>
List the files in the database.
<br><br>


### Command Syntax
`files-list [max=INT] [PRESENTATION_FLAGS]`<br>
`max` - The number of the maximum files to list.<br>
`PRESENTATION_FLAGS` - common presentation flags for the SparkCli.<br>
For more info on presentation flags, check the [Presentation flags manual](/listiary/wiki/spark/v05/pflags/).
<br><br>



### Examples
`php spark.php files-list`<br>
List all the files in the database.
<br><br>
`php spark.php files-list max=10`<br>
List the first 10 files in the database.
<br><br>
`php spark.php files-list theme=DEFAULT`<br>
List all the files in the database, with presentation flags.
<br><br>
`php spark.php files-list -hb theme=DEFAULT`<br>
List all the files in the database, with presentation flags.
<br><br>
`php spark.php files-list -auto -hb theme=DEFAULT`<br>
List all the files in the database, with presentation flags.
<br><br>


### Links
[Back](/listiary/wiki/spark/v05/)