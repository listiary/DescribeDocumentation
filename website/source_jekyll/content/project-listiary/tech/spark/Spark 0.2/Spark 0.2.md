---
layout: page
title: Listiary Spark v0.2
permalink: /listiary/wiki/spark/v02/
exclude: true
---
Spark 0.2 started to form more like a proper collection of command line tools.
It was also developed on my Linux Mint machine, to be used from the terminal.
<br><br>

_N.B. Spark 0.2 was created for an older version of the database, and running it against a modern Listiary database will not be safe - it is provided as a curiosity._
<br><br>


## Scripts

In the scripts below, whenever we say something about the database for example - that comes from the file named `_config.php` - the config to be used. That file holds the constants that tell the script what database to connect to.
<br><br>

`_config.php` - The config to be used.<br>
`_config_template.php` - The template used in creating the config to be used.
<br><br>

`1list_files.php` - List all files in a selected dir on the local file system.<br>
`1set_config.php` - Create a config file for the Listiary database.<br>
`1create_tables.php` - Create the needed tables for the wiki in the database.<br>
`1wipe_database.php` - Delete all the contents from a database - as means to uninstall the wiki.
<br><br>

`2upload_files.php` - Upload all the files from a given dir to the database.<br>
`2upload_file.php` - Upload a single file to the database.<br>
`2download_files.php` - Download all the files from the database to a local dir.<br>
`2download_file.php` - Download a selected file from the database to a local dir.<br>
`2delete_files.php` - Delete all the files from the database.<br>
`2delete_file.php` - Delete a file from the database.<br>
`2list_files.php` - List all the files in the database.
<br><br>

`3compile_database.php` - No original Documentation. Compile the whole database.<br>
`3compile_entry.php` - No original Documentation. Compile an entry.
<br><br>

`4curate_database_filenames.php` - No original Documentation. Create the filename metadata.<br>
`4curate_database_ids.php` - No original Documentation. Create the id metadata.
<br><br>


### Script Examples

[1list_files.php](/listiary/wiki/spark/v02/example11/)<br>
[1set_config.php](/listiary/wiki/spark/v02/example12/)<br>
[1create_tables.php](/listiary/wiki/spark/v02/example13/)<br>
[1wipe_database.php](/listiary/wiki/spark/v02/example14/)<br>
<br>
[2upload_files.php](/listiary/wiki/spark/v02/example21/)<br>
[2upload_file.php](/listiary/wiki/spark/v02/example22/)<br>
[2download_files.php](/listiary/wiki/spark/v02/example23/)<br>
[2download_file.php](/listiary/wiki/spark/v02/example24/)<br>
[2delete_files.php](/listiary/wiki/spark/v02/example25/)<br>
[2delete_file.php](/listiary/wiki/spark/v02/example26/)<br>
[2list_files.php](/listiary/wiki/spark/v02/example27/)<br>
<br>

	
### Links
[Back](/listiary/wiki/spark/)