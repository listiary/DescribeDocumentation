---
layout: page
title: files-upload
permalink: /listiary/wiki/spark/v05/files-upload/
exclude: true
---
<br>
Upload Describe files to the database.
<br>
The user copies the files to upload in the `_uploads` directory,
puting them inside a folder, gives that relative path to the function,
and the files get uploaded to the database.
<br>
For example, user that runs : `php spark.php file-upload "files-1"`<br>
will get those files in the database
<br><br>



### Command Syntax
`files-upload [PRESENTATION_FLAGS]`<br>
`PRESENTATION_FLAGS` - common presentation flags for the SparkCli.<br>
For more info on presentation flags, check the [Presentation flags manual](/listiary/wiki/spark/v05/pflags/).
<br><br>



### Examples
`php spark.php files-upload "uploads-1"`<br>
Upload files to the database.
<br><br>
`php spark.php files-upload "uploads-1" theme=DEFAULT`<br>
Upload files to the database, with presentation flags.
<br><br>
`php spark.php files-upload "uploads-1" -hb theme=DEFAULT`<br>
Upload files to the database, with presentation flags.
<br><br>
`php spark.php files-upload "uploads-1" -auto -hb theme=DEFAULT`<br>
Upload files to the database, with presentation flags.
<br><br>


### Links
[Back](/listiary/wiki/spark/v05/)