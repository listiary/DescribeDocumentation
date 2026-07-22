---
layout: page
title: 2upload_files
permalink: /listiary/wiki/spark/v02/example21/
exclude: true
---
Upload all the files from a given directory to the database specified in the `_config.php`.
<br><br>


### Usage
`php 2upload_files.php "/path/to/directory"`<br>
usage (bash) - output to console<br>

`php 2upload_files.php "/path/to/directory" > "output.txt"`<br>
usage (bash) - output to file<br>

`php 2upload_files.php "/path/to/directory" >> "output.txt"`<br>
usage (bash) - append to file<br>

`php 2upload_files.php "/path/to/directory" 2> "errors.txt"`<br>
usage (bash) - capture errors to file<br>

`php 2upload_files.php "/path/to/directory" 2>> "errors.txt"`<br>
usage (bash) - append errors to file<br>

`php 2upload_files.php "/path/to/directory" > "all_output.txt" 2>&1`<br>
usage (bash) - capture output and errors to file<br>

`php 2upload_files.php "/path/to/directory" &> "all_output.txt"`<br>
usage (bash 4+) - capture output and errors to file<br>
<br><br>


### Links
[Back](/listiary/wiki/spark/v02/)