---
layout: page
title: Listiary Spark v0.3
permalink: /listiary/wiki/spark/v03/
exclude: true
---
Spark 0.3 continued to build on what 0.2 started - a collection of command line tools. It was developed on Windows 11, to be used from the CMD console.
<br><br>
This version added some file structure as well. The `_configs` folder now was the place where configs were stored, so that we can juggle few of them more easily. We also have a `_downloads` folder - the default place where downloaded content end up at.
<br><br>
Structurally, we now have wrapper scripts that we execute from the command line, and library files that contain the core functionality, inside the `tasks` and `utils` folders. This starts to look like a CLI runner and a backend library starting to form, but we won't have that until v 0.5
<br><br>


### Scripts

`config_show.php` - Show the constants inside the selected config.<br>
`config_test.php` - Test the selected config against the backend server.<br>
<br>

`database_curate_filenames.php` - Generate the metadata for all the files, populating 1 of the 2 tables.<br>
`database_curate_ids.php` - Generate the metadata for all the files, populating 1 of the 2 tables.<br>
`database_make_tables.php` - Make the tables in an empty database, installing a wiki instance.<br>
`database_test.php` - Test if database is working and empty for Listiary installation.<br>
`database_wipe.php` - Nuke a database, deleting everything from it.<br>
<br>

`files_compile.php` - Compile all Describe files in the database, populating the JSONs table.<br>
`files_count.php` - Count the files in the database.<br>
`files_delete.php` - Delete all the Describe files from the database.<br>
`files_delete_nowarn.php` - Delete all the Describe files from the database, don't ask for confirmation.<br>
`files_download.php` - Download Describe files from the database.<br>
`files_list.php` - List the files in the database.<br>
`files_upload.php` - Upload Describe files to the database.<br>
<br>

`file_compile.php` - Compile a single file in the database to JSON.<br>
`file_delete.php` - Delete a single file.<br>
`file_delete_nowarn.php` - Delete a single file, don't ask for confirmation.<br>
`file_download.php` - Download a Describe file.<br>
`file_upload.php` - Upload a Describe file to the database.<br>
`file_view.php` - Output the contents of a single file.<br>
<br>

`jsons_count.php` - Count the JSON files in the database.<br>
`jsons_delete.php` - Delete all the JSON files from the database.<br>
`jsons_delete_nowarn.php` - Delete all the JSON files from the database, don't ask for confirmation.<br>
`jsons_download.php` - Download JSON files from the database.<br>
`jsons_list.php` - List the JSON files in the database.<br>
`jsons_upload.php` - Upload JSON files to the database.<br>
<br>

`json_delete.php` - Delete a single JSON file.<br>
`json_delete_nowarn.php` - Delete a single JSON file, don't ask for confirmation.<br>
`json_download.php` - Download a JSON file.<br>
`json_upload.php` - Upload given data representing a JSON file to the database.<br>
`json_view.php` - Output the contents of a single json file.<br>
<br>

`metadataff_view.php` - Output the contents of a metadata entry. FF metadata - File to Files.<br>
`metadatafi_view.php` - Output the contents of a metadata entry. FI metadata - File to item Ids.<br>
`metadataif_view.php` - Output the contents of a metadata entry. IF metadata - Item Id to Files.<br>
<br><br>


### Links
[Back](/listiary/wiki/spark/)