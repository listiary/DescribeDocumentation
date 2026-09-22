---
layout: page
title: TestTodo - SparkLib - Download-Upload
permalink: /listiary/articles/wjpntagofq/
exclude: true
---
<br>
```
Article type: Test Todo
Article name: TestTodo - SparkLib - Download-Upload
Affected Software/module: SparkLib, SparlCli
Author:	Framez
```
<br><br>

## Description:
We need to test the output of our database download function against the one executed from PhpMyAdmin.
I suggest we do that by using our output to import to an empty database, then using the PhpMyAdmin output
to do the same, then using PhpMyAdmin to export the two databases and compare the resulted export SQL, or
alternatively - use some other method to compare the 2 databases, or the two export SQL files.
<br><br>

## Relevant commands:
```
php spark.php config-make
php spark.php config-test
php spark.php database-download
php spark.php database-upload "database-sql-dump.sql"
```

<br><br>
### Links
[Back](/listiary/articles/)<br>