---
layout: page
title: Listiary Spark v0.5
permalink: /listiary/wiki/spark/v05/
exclude: true
---
Spark 0.5 is a rewrite of Spark 0.4 in a Cli tool and Library format.
Now, we have one tool that is the Cli runner - SparkCli, and the library that can be reused across other projects - SparkLib.
<br><br>
Spark is an administrative CLI interface for administering the Listiary database layer. Spark is very powerful and unforgiving - be careful which script you are invoking and read the documentation.<br>
Spark is licensed under [GNU Affero General Public License, version 3 (AGPLv3)](https://www.gnu.org/licenses/agpl-3.0.html).<br>
For more information visit [documentation.listiary.org/listiary/wiki/spark/](https://documentation.listiary.org/listiary/wiki/spark/).
<br><br>

### List of articles
[Spark 0.5 - Misc](/listiary/wiki/spark/v05/misc/) - The help command and more.<br>
[Spark 0.5 - Presentation flags](/listiary/wiki/spark/v05/flags/) - The presentation flags for functions.<br>
[Spark 0.5 - Configs](/listiary/wiki/spark/v05/configs/) - How SparkCli deals with Listiary configs.<br>
[Spark 0.5 - REPL](/listiary/wiki/spark/v05/repl/) - REPL and no-repl functions in SparkCli 0.5.<br>
[Spark 0.5 - Files and Jsons](/listiary/wiki/spark/v05/fjfuncs/) - Raw Describe file operations on the database.<br>
[Spark 0.5 - Metadata](/listiary/wiki/spark/v05/mfuncs/) - Metadata operations on the database.<br>
[Spark 0.5 - Database and Action](/listiary/wiki/spark/v05/dafuncs/) - Functions that deal with the database as a whole.
<br><br>


### List of commands

[`NONE`](/listiary/wiki/spark/v05/none/) - This is running the SparkCli without any arguments. Will output the help message.<br>
[`UNKNOWN`](/listiary/wiki/spark/v05/none/) - This is running the SparkCli with some invalid first argument. Will output the help message.<br>
[`PRESENTATION_FLAGS`](/listiary/wiki/spark/v05/pflags/) - Presentation flags for the functions.<br>
[`help`](/listiary/wiki/spark/v05/help/) - Output the help message.
<br><br>

[`config-make`](/listiary/wiki/spark/v05/config-make/) - Make a config file, by asking the user to input values on the CMD.<br>
[`config-make-online`](/listiary/wiki/spark/v05/config-make-online/) - Make a config file. Test connection and credentials.<br>
[`config-make-offline`](/listiary/wiki/spark/v05/config-make-offline/) - Make a config file. Don't test connection and credentials.<br>
[`configs-list`](/listiary/wiki/spark/v05/configs-list/) - List all the configs in the `_configs` folder.<br>
[`config-show`](/listiary/wiki/spark/v05/config-show/) - Show the constants inside the selected config.<br>
[`config-test`](/listiary/wiki/spark/v05/config-test/) - Test the selected config against the backend server.<br>
[`config-test-compiler`](/listiary/wiki/spark/v05/config-test-compiler/) - Test the compiler service for the current config.
<br><br>

[`action-create-stub`](/listiary/wiki/spark/v05/action-create-stub/) - Create a new article stub.<br>
[`action-delete-article`](/listiary/wiki/spark/v05/action-delete-article/) - Delete an article and all its files.
<br><br>

[`database-test`](/listiary/wiki/spark/v05/database-test/) - Test if database is working and empty for Listiary installation.<br>
[`database-make-tables`](/listiary/wiki/spark/v05/database-make-tables/) - Make the tables in an empty database, installing a wiki instance.<br>
[`database-wipe`](/listiary/wiki/spark/v05/database-wipe/) - Nuke a database, deleting everything from it.<br>
[`database-download`](/listiary/wiki/spark/v05/database-download/) - Download a copy of the database.<br>
[`database-upload`](/listiary/wiki/spark/v05/database-upload/) - Upload a copy of the database.<br>
[`database-recompile`](/listiary/wiki/spark/v05/database-recompile/) - Recompile all the files in the database.<br>
[`database-curate`](/listiary/wiki/spark/v05/database-curate/) - Generate the full metadata for all the files.<br>
[`database-curate-ids`](/listiary/wiki/spark/v05/database-curate-ids/) - Generate the metadata for all the files, populating 1 of the 2 tables.<br>
[`database-curate-filenames`](/listiary/wiki/spark/v05/database-curate-filenames/) - Generate the metadata for all the files, populating 1 of the 2 tables.<br>
[`database-find-orphans`](/listiary/wiki/spark/v05/database-find-orphans/) - Find orphaned articles in the database.
<br><br>

[`file-view`](/listiary/wiki/spark/v05/file-view/) - Output the contents of a single file.<br>
[`file-download`](/listiary/wiki/spark/v05/file-download/) - Download a Describe file.<br>
[`file-upload`](/listiary/wiki/spark/v05/file-upload/) - Upload a Describe file to the database.<br>
[`file-compile`](/listiary/wiki/spark/v05/file-compile/) - Compile a single file in the database to JSON.<br>
[`file-delete`](/listiary/wiki/spark/v05/file-delete/) - Delete a single file.
<br><br>

[`files-list`](/listiary/wiki/spark/v05/files-list/) - List the files in the database.<br>
[`files-count`](/listiary/wiki/spark/v05/files-count/) - Count the files in the database.<br>
[`files-download`](/listiary/wiki/spark/v05/files-download/) - Download Describe files from the database.<br>
[`files-upload`](/listiary/wiki/spark/v05/files-upload/) - Upload Describe files to the database.<br>
[`files-compile`](/listiary/wiki/spark/v05/files-compile/) - Compile all Describe files in the database, populating the JSONs table.<br>
[`files-delete`](/listiary/wiki/spark/v05/files-delete/) - Delete all the Describe files from the database.
<br><br>

[`json-view`](/listiary/wiki/spark/v05/json-view/) - Output the contents of a single json file.<br>
[`json-download`](/listiary/wiki/spark/v05/json-download/) - Download a JSON file.<br>
[`json-upload`](/listiary/wiki/spark/v05/json-upload/) - Upload given data representing a JSON file to the database.<br>
[`json-delete`](/listiary/wiki/spark/v05/json-delete/) - Delete a single JSON file.
<br><br>

[`jsons-list`](/listiary/wiki/spark/v05/jsons-list/) - List the JSON files in the database.<br>
[`jsons-count`](/listiary/wiki/spark/v05/jsons-count/) - Count the JSON files in the database.<br>
[`jsons-download`](/listiary/wiki/spark/v05/jsons-download/) - Download JSON files from the database.<br>
[`jsons-delete`](/listiary/wiki/spark/v05/jsons-delete/) - Delete all the JSON files from the database.
<br><br>

[`metadata-view`](/listiary/wiki/spark/v05/metadata-view/) - Output the contents of a single metadata entry.
<br><br>


### Links
[Back](/listiary/wiki/spark/)