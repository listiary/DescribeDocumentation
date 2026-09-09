---
layout: page
title: Database - Main
permalink: /listiary/wiki/database/main/
exclude: true
---
<br>
These are the tables in the database where Listiary stores all the articles. We have 2 tables - one for raw Describe documents, that users can edit, and another for compiled documents that the wiki uses. Or - `describe_documents` and `compiled_documents` respectively. `describe_documents` holds the Describe source files, and `compiled_documents` - the compiled versions of those files in JSON.<br><br>
There are also indexes for each of those tables - `idx_filename`, so that we can quickly search by filename.
<br><br>

```
describe_documents
  .id
  .filename
  .content
  .submitted_at
  
compiled_documents
  .id
  .filename
  .content
  .submitted_at
```
<br>
<br>

### Links
[Versioning](/listiary/wiki/database/versioning/)<br>
[Subsystems - Metadata (Housekeeping)](/listiary/wiki/database/metadata/)<br>
[Subsystems - Edit history](/listiary/wiki/database/history/)<br>
[Subsystems - Accounts](/listiary/wiki/database/accounts/)<br>
[Subsystems - Permissions (Authorization)](/listiary/wiki/database/auth/)<br>
<br>
[Listiary Wiki - Database](/listiary/wiki/database/)<br>
[Listiary Wiki - Repo map](/listiary/wiki/repo-map/)<br>
[Back](/listiary/wiki/)
