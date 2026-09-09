---
layout: page
title: Database - Permissions
permalink: /listiary/wiki/database/auth/
exclude: true
---
<br>
This subsystem is responsible for permissions management in the wiki - or who is allowed to access, edit, read etc. what. This is also called Authorization.<br>
A user is authenticated when he logs in, and then authorized to access a particular resource.<br>
<br><br>

### Account Roles
The `permissions_account_roles` table defines which user has what role.<br>
The roles users can have are: `USER_VIEWER`, `USER_EDITOR`, `USER_SPONSOR`, `USER_MODERATOR`, `USER_ADMIN`, `USER_GOD`<br><br>
<span style="color:blue">**_account_id_**</span> - the id of the user account.<br>
<span style="color:blue">**_account_role_**</span> - the role the user has in the wiki.<br>
<br><br>

### Permissions per Item per User
Users can have different roles for their account, and those dictate what they can do on all unrestricted items, articles, etc.<br>
But items like articles or namespaces can also have specific permissions per user (or user group).<br>
So, for example, an item can be restricted to a specific user, or a specific user can be given permission to edin a specific resource.<br><br>
<span style="color:blue">**_id_**</span> - id of the item<br>
<span style="color:blue">**_resource_type_**</span> - the type of the resource being accessed: `ARTICLE`<br>
<span style="color:blue">**_resource_id_**</span> - the id of the resource or article for example<br>
<span style="color:blue">**_account_id_**</span> - the id of the user in question<br>
<span style="color:blue">**_permission_level_**</span> - what this user is allowed to do: `READ`, `WRITE`, `MANAGE`<br>
<br><br>

### Permissions per Item per Role
What user role can access what item and do what with it.<br><br>
<span style="color:blue">**_id_**</span> - id of the item<br>
<span style="color:blue">**_resource_type_**</span> - the type of the resource being accessed: `ARTICLE`<br>
<span style="color:blue">**_resource_id_**</span> - the id of the resource or article for example<br>
<span style="color:blue">**_account_role_**</span> - the role the user has in the wiki. The roles users can have are: `USER_VIEWER`, `USER_EDITOR`, `USER_SPONSOR`, `USER_MODERATOR`, `USER_ADMIN`, `USER_GOD`<br>
<span style="color:blue">**_permission_level_**</span> - what this user is allowed to do: `READ`, `WRITE`, `MANAGE`<br>

<br><br>

```
permissions_account_roles 
  .account_id
  .account_role

permissions_resource_accounts
  .id
  .resource_type
  .resource_id
  .account_id
  .permission_level

permissions_resource_roles
  .id
  .resource_type
  .resource_id
  .account_role
  .permission_level
```
<br>
<br>

### Links
[Versioning](/listiary/wiki/database/versioning/)<br>
[Subsystems - Main Data](/listiary/wiki/database/main/)<br>
[Subsystems - Metadata (Housekeeping)](/listiary/wiki/database/metadata/)<br>
[Subsystems - Edit history](/listiary/wiki/database/history/)<br>
[Subsystems - Accounts](/listiary/wiki/database/accounts/)<br>
<br>
[Listiary Wiki - Database](/listiary/wiki/database/)<br>
[Listiary Wiki - Repo map](/listiary/wiki/repo-map/)<br>
[Back](/listiary/wiki/)
