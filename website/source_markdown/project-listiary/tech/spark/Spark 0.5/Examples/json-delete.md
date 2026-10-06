---
layout: page
title: json-delete
permalink: /listiary/wiki/spark/v05/json-delete/
exclude: true
---
<br>
Delete a single JSON file in the database.
<br>
The user runs a command like `jsons-list` to list the json files in the database,
then runs `json-delete` to delete a single json file.
<br><br>


### Command Syntax
`json-delete FILE_NAME [PRESENTATION_FLAGS]`<br>
`FILE_NAME` - The name of the json file in the database.<br>
`PRESENTATION_FLAGS` - common presentation flags for the SparkCli.<br>
For more info on presentation flags, check the [Presentation flags manual](/listiary/wiki/spark/v05/pflags/).
<br><br>



### Examples
`php spark.php json-delete "root.name"`<br>
Delete a json file
<br><br>
`php spark.php json-delete "root.name" theme=DEFAULT`<br>
Delete a json file with presentation flags
<br><br>
`php spark.php json-delete "root.name" -hb theme=DEFAULT`<br>
Delete a json file with presentation flags
<br><br>
`php spark.php json-delete "root.name" -auto -hb theme=DEFAULT`<br>
Delete a json file with presentation flags
<br><br>


### Links
[Back](/listiary/wiki/spark/v05/)