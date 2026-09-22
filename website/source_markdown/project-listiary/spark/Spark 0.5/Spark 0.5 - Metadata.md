---
layout: page
title: Spark v0.5 - Metadata
permalink: /listiary/wiki/spark/v05/mfuncs/
exclude: true
---
<br>
Listiary database contains and keeps metadata for the contents of different files.
This is needed for proper prefetching of data and is needed for the correct work of the wiki.
<br><br>
FF metadata stands for File to Files. It describes what other files each file is related to.<br>
FI metadata stands for File to item Ids. It describes what files contain each public item Id.<br>
IF metadata stands for item Id to Files. It describes what files contain each public item Id.<br>
<br><br>



### Functions
[`metadata-view`](/listiary/wiki/spark/v05/metadata-view/) - Output the contents of a single metadata entry.
<br>
```
php spark.php metadata-view ff "FILE_NAME"
php spark.php metadata-view fi "FILE_NAME"
php spark.php metadata-view if "ITEM_ID"
```
<br><br>


### Links
[Back](/listiary/wiki/spark/v05/)