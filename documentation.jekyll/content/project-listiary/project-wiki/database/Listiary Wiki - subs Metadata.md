---
layout: page
title: Database - Metadata
permalink: /listiary/wiki/database/metadata/
exclude: true
---
<br>
These are metadata for the files in the wiki - so that Listiary knows which compiled JSON files to prefetch and which to render.<br><br>
<span style="color:blue">**_housekeeping_itemid_filename_**</span> - table links Describe item ids to filenames they are defined in.<br>
<span style="color:blue">**_housekeeping_filename_related_**</span> - table links files to files needed when loading them.<br>
<br><br>

```
housekeeping_itemid_filename
  .filename
  .item_id

housekeeping_filename_related
  .filename
  .related_filename
```
<br>
<br>

### Links
[Versioning](/listiary/wiki/database/versioning/)<br>
[Subsystems - Main Data](/listiary/wiki/database/main/)<br>
[Subsystems - Edit history](/listiary/wiki/database/history/)<br>
[Subsystems - Accounts](/listiary/wiki/database/accounts/)<br>
[Subsystems - Permissions (Authorization)](/listiary/wiki/database/auth/)<br>
<br>
[Listiary Wiki - Database](/listiary/wiki/database/)<br>
[Listiary Wiki - Repo map](/listiary/wiki/repo-map/)<br>
[Back](/listiary/wiki/)
