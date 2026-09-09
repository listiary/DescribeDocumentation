---
layout: page
title: 2delete_file
permalink: /listiary/wiki/spark/v02/example26/
exclude: true
---
Delete a file from the database (One that we connect to in our `_config.php`).
<br><br>


### Usage
`php 2delete_file.php "name.in.database"`<br>
usage (bash) - output to console<br>

`php 2delete_file.php "name.in.database" > "output.txt"`<br>
usage (bash) - output to file<br>

`php 2delete_file.php "name.in.database" >> "output.txt"`<br>
usage (bash) - append to file<br>

`php 2delete_file.php "name.in.database" 2> "errors.txt"`<br>
usage (bash) - capture errors to file<br>

`php 2delete_file.php "name.in.database" 2>> "errors.txt"`<br>
usage (bash) - append errors to file<br>

`php 2delete_file.php "name.in.database" > "all_output.txt" 2>&1`<br>
usage (bash) - capture output and errors to file<br>

`php 2delete_file.php "name.in.database" &> "all_output.txt"`<br>
usage (bash 4+) - capture output and errors to file<br>
<br><br>


### Links
[Back](/listiary/wiki/spark/v02/)