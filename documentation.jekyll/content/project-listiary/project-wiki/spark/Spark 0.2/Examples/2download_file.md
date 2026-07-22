---
layout: page
title: 2download_file
permalink: /listiary/wiki/spark/v02/example24/
exclude: true
---
Download a selected file from the database (from the `_config.php`) to a local directory.
<br><br>


### Usage
`php 2download_file.php "name.in.database" "/path/to/directory"`<br>
usage (bash) - output to console<br>

`php 2download_file.php "name.in.database" "/path/to/directory" > "output.txt"`<br>
usage (bash) - output to file<br>

`php 2download_file.php "name.in.database" "/path/to/directory" >> "output.txt"`<br>
usage (bash) - append to file<br>

`php 2download_file.php "name.in.database" "/path/to/directory" 2> "errors.txt"`<br>
usage (bash) - capture errors to file<br>

`php 2download_file.php "name.in.database" "/path/to/directory" 2>> "errors.txt"`<br>
usage (bash) - append errors to file<br>

`php 2download_file.php "name.in.database" "/path/to/directory" > "all_output.txt" 2>&1`<br>
usage (bash) - capture output and errors to file<br>

`php 2download_file.php "name.in.database" "/path/to/directory" &> "all_output.txt"`<br>
usage (bash 4+) - capture output and errors to file<br>
<br><br>


### Links
[Back](/listiary/wiki/spark/v02/)