---
layout: page
title: jsons-list
permalink: /listiary/wiki/spark/v05/jsons-list/
exclude: true
---
List the JSON files in the database.
<br><br>


### Command Syntax
`jsons-list [max=INT] [PRESENTATION_FLAGS]`<br>
`max` - The number of the maximum files to list.<br>
`PRESENTATION_FLAGS` - common presentation flags for the SparkCli.<br>
For more info on presentation flags, check the [Presentation flags manual](/listiary/wiki/spark/v05/pflags/).
<br><br>



### Examples
`php spark.php jsons-list`<br>
List all the compiled JSON files in the database.
<br><br>
`php spark.php jsons-list max=10`<br>
List the first 10 compiled JSON files in the database.
<br><br>
`php spark.php jsons-list theme=DEFAULT`<br>
List all the compiled JSON files in the database, with presentation flags.
<br><br>
`php spark.php jsons-list -hb theme=DEFAULT`<br>
List all the compiled JSON files in the database, with presentation flags.
<br><br>
`php spark.php jsons-list -auto -hb theme=DEFAULT`<br>
List all the compiled JSON files in the database, with presentation flags.
<br><br>


### Links
[Back](/listiary/wiki/spark/v05/)