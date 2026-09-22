---
layout: page
title: database-test
permalink: /listiary/wiki/spark/v05/database-test/
exclude: true
---
<br>
Test if database is working and empty for Listiary installation.
<br><br>
User have made an empty database, set up an user for it,
then he runs a command like `config-make`, and provides the data, to create the config,
then the user runs `database-test`, to make sure the database is suitable for installing a Listiary instance.
<br><br>
This command is used when installing a new Listiary wiki.
<br><br>


### Command Syntax

`database-test [PRESENTATION_FLAGS]`<br>
`PRESENTATION_FLAGS` - common presentation flags for the SparkCli.<br>
For more info on presentation flags, check the [Presentation flags manual](/listiary/wiki/spark/v05/pflags/).
<br><br>



### Examples
`php spark.php database-test`<br>
Test a database for wiki installation.
<br><br>
`php spark.php database-test theme=DEFAULT`<br>
Test a database for wiki installation with presentation flags
<br><br>
`php spark.php database-test -hb theme=DEFAULT`<br>
Test a database for wiki installation with presentation flags
<br><br>
`php spark.php database-test -auto -hb theme=DEFAULT`<br>
Test a database for wiki installation with presentation flags
<br><br>


### Links
[Back](/listiary/wiki/spark/v05/)