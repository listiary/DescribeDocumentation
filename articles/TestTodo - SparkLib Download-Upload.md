Article type: 						`Test Todo`<br>
Article name:						`TestTodo - SparkLib Download-Upload`<br>
Affected Software/module:			`SparkLib`, `SparlCli`<br>
Author:								`Framez`<br>
<br>

## Description:
We need to test the output of our database download function against the one executed from PhpMyAdmin.
I suggest we do that by using our output to import to an empty database, then using the PhpMyAdmin output
to do the same, then using PhpMyAdmin to export the two databases and compare the resulted export SQL, or
alternatively - use some other method to compare the 2 databases, or the two export SQL files.

## Relevant commands:
```
php spark.php config-make
php spark.php config-test
php spark.php database-download
php spark.php database-upload "database-sql-dump.sql"
```