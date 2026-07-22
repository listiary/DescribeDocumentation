---
layout: page
title: files-compile
permalink: /listiary/wiki/spark/v05/files-compile/
exclude: true
---
<br>
Compile/recompile the files in the database.
<br><br>


### Command Syntax
`files-compile [PRESENTATION_FLAGS]`<br>
`PRESENTATION_FLAGS` - common presentation flags for the SparkCli.<br>
For more info on presentation flags, check the [Presentation flags manual](/listiary/wiki/spark/v05/pflags/).
<br><br>



### Examples
`php spark.php files-compile`<br>
Compile all the files in the database.
<br><br>
`php spark.php files-compile theme=DEFAULT`<br>
Compile all the files in the database, with presentation flags.
<br><br>
`php spark.php files-compile -hb theme=DEFAULT`<br>
Compile all the files in the database, with presentation flags.
<br><br>
`php spark.php files-compile -auto -hb theme=DEFAULT`<br>
Compile all the files in the database, with presentation flags.
<br><br>


### Links
[Back](/listiary/wiki/spark/v05/)