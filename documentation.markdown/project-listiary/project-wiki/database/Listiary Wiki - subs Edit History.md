---
layout: page
title: Database - Edit History
permalink: /listiary/wiki/database/history/
exclude: true
---
<br>
We have added an edit history system some time before, as any real wiki needs one. When users edit an article, it creates a new entry in the `document_versions` table. `document_versions` is the table responsible for keeping the edit history in the wiki. We can store this edit in the form of Text and Json artifacts in the table - so bigger footprint, but fast retrieval, or we can later choose to antiquate the item - which we will do with database management tools like Spark. We can store a version as text only, as text and json, and as delta only - depending on how fast we want to be able to restore the item versus how much space it will take to store in the DB. Probably older changes will be pruned to include only the delta, and newer will be stored in full. An antiquated item stores only the delta of the edit, thus reducing the storage space needed. And every entry in this table holds a reference to the previous edit and the next edit - so we can reconstruct history.
<br><br>

<span style="color:blue">**_text_**</span> -  is the text version of the describe document - that is, the article.<br>
<span style="color:blue">**_json_**</span> -  is the compiled JSON version the describe document - that is, the article.<br>
<span style="color:blue">**_delta_**</span> -  is the difference between the previous version and this one.<br>
<span style="color:blue">**_edit_comment_**</span> - the edit comment. Comment is a reserved word in SQL, by the way.<br>
<span style="color:blue">**_is_minor_**</span> - whether the edit is a minor one.<br>
<span style="color:blue">**_document_id_**</span> - links to the document id in the `describe_documents` table.<br>
<span style="color:blue">**_previous_version_id_**</span> - link to the previous edit item, in a linked list fashion.<br>
<span style="color:blue">**_next_version_id_**</span> - link to the next edit item, in a linked list fashion.<br>
<span style="color:blue">**_usercode_**</span> - the user who created the edit.<br>
<span style="color:blue">**_created_at_**</span> - time of creation.<br>
<span style="color:blue">**_antiquated_at_**</span> - when was the newer edit created - or basically when this edit became not the latest one.<br>
<br><br>

```
document_versions
  .id

  .text
  .json
  .delta

  .comment
  .is_minor

  .document_id
  .previous_version_id
  .next_version_id

  .usercode
  .created_at
  .antiquated_at
```
<br>
<br>

### Links
[Versioning](/listiary/wiki/database/versioning/)<br>
[Subsystems - Main Data](/listiary/wiki/database/main/)<br>
[Subsystems - Metadata (Housekeeping)](/listiary/wiki/database/metadata/)<br>
[Subsystems - Accounts](/listiary/wiki/database/accounts/)<br>
[Subsystems - Permissions (Authorization)](/listiary/wiki/database/auth/)<br>
<br>
[Listiary Wiki - Database](/listiary/wiki/database/)<br>
[Listiary Wiki - Repo map](/listiary/wiki/repo-map/)<br>
[Back](/listiary/wiki/)
