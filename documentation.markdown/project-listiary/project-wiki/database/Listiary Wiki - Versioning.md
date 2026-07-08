---
layout: page
title: Database - Versioning
permalink: /listiary/wiki/database/versioning/
exclude: true
---
<br>
In Listiary, subsystems are versioned internally - like separate pieces of software that come together - which they kind of are, in all fairness.<br>
Currently, the database is in version 0.3.1<br><br>

### v 0.1 - Initial
<span style="color:blue">**_Main data_**</span> - staged_documents, compiled_documents, accounts<br>
_The accounts table is a simple dummy one - accounts were not properly implemented_
<br><br>

### v 0.2 - More sophistication
<span style="color:blue">**_Main data_**</span> - describe_documents, compiled_documents<br>
<span style="color:blue">**_Metadata_**</span> - housekeeping_itemid_filename, housekeeping_filename_related<br>
<span style="color:blue">**_Accounts_**</span> - accounts<br>
_We have added metadata for the stored documents, so the wiki can easily navigate them._
_Accounts are still dummy._
<br><br>

### v 0.3 - Fully implemented accounts
<span style="color:blue">**_Main data_**</span> - describe_documents, compiled_documents<br>
<span style="color:blue">**_Metadata_**</span> - housekeeping_itemid_filename, housekeeping_filename_related<br>
<span style="color:blue">**_Edit history_**</span> - document_versions<br>
<span style="color:blue">**_Accounts_**</span> - accounts, account_details, persistent_logins<br>
<span style="color:blue">**_Authentication_**</span> - password_resets, login_attempts, register_success, password_reset_resends<br>
<span style="color:blue">**_Authorization_**</span> - permissions_account_roles, permissions_resource_accounts, permissions_resource_roles<br>
_We have been working on properly implementing accounts in the wiki - or Authentication and Authorization, as it is known in security contexts_
<br><br>

### v 0.3.1 - slight table renaming
_Some slight renaming of few indexes, otherwise - the same thing_

<br>
<br>

### Links
[Subsystems - Main Data](/listiary/wiki/database/main/)<br>
[Subsystems - Metadata (Housekeeping)](/listiary/wiki/database/metadata/)<br>
[Subsystems - Edit history](/listiary/wiki/database/history/)<br>
[Subsystems - Accounts](/listiary/wiki/database/accounts/)<br>
[Subsystems - Permissions (Authorization)](/listiary/wiki/database/auth/)<br>
<br>
[Listiary Wiki - Database](/listiary/wiki/database/)<br>
[Listiary Wiki - Repo map](/listiary/wiki/repo-map/)<br>
[Back](/listiary/wiki/)
