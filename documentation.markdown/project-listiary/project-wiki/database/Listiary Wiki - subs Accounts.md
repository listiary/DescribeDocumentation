---
layout: page
title: Database - Accounts
permalink: /listiary/wiki/database/accounts/
exclude: true
---
<br>
This subsystem involves all the tables needed for authorization and authentication - actions connected to accounts.<br>
But also there are tables related to the account system, that handle temporary tokens, persistent login tokens, rate limiters, etc.<br>
The accounts table is the main one.<br>
<br><br>

### Accounts
<span style="color:blue">**_id_**</span> - every user has unique account id.<br>
<span style="color:blue">**_username_**</span> - the user's username<br>
<span style="color:blue">**_email_**</span> - the user's email<br>
<span style="color:blue">**_usercode_**</span> - don't know if we need to remove this, when we have a user id, but it is an unique code for each user - like a hash<br>
<span style="color:blue">**_password_hash_**</span> - the hash of the password<br>
<br>
<span style="color:blue">**_is_bot_**</span> - boolean - whether the account is a bot or a human<br>
<span style="color:blue">**_is_active_**</span> - boolean - whether the account is activated (email has been verified)<br>
<span style="color:blue">**_is_premium_**</span> - boolean - whether the account is a paid or a free one. Paid accounts enjoy additional perks.
<br>
<span style="color:blue">**_created_at_**</span> - account creation timestamp<br>
<span style="color:blue">**_verification_token_**</span> - this token is present while the account is still not activated.<br>
Activation removes the record - as we don't need it any more.<br>
<br>

```
accounts
  .id
  .username
  .email
  .usercode
  .password_hash
  .is_bot
  .is_active
  .is_premium
  .created_at
  .verification_token
```
<br><br>

### Account Details
`account_id` - every user has unique account id. It links this table to the previous one.<br>


**_Avatar related_**<br>
We support few different, customize-able avatar shapes.<br>
<span style="color:blue">**_avatar_path_**</span> - The path of the avatar file. At the moment, we are uploading avatars on the server.<br>
<span style="color:blue">**_avatar_shape_**</span> - The shape word - like triangle or square. We allow different avatar shapes.<br>
<span style="color:blue">**_avatar_shape_radius_**</span> - The angle radius of the avatar shape.<br>
<span style="color:blue">**_avatar_updated_at_**</span> - The date when the avatar was updated last.<br>
<br>
**_Profile fields_**<br>
We have floated the idea about having multiple biographies with a likelihood to show one, in percents.<br>
<span style="color:blue">**_bio_**</span> - The user's biography<br>
<span style="color:blue">**_city_**</span> - The user's place of residence<br>
<span style="color:blue">**_country_**</span> - The user's country of residence<br>
<span style="color:blue">**_timezone_**</span> - The user's timezone.<br>
<br>
**_Social links_**<br>
<span style="color:blue">**_link_personal_website_**</span> - User's personal website URL<br>
<span style="color:blue">**_link_personal_facebook_**</span> - User's facebook account URL<br>
<span style="color:blue">**_link_personal_xcom_**</span> - User's x.com account URL<br>
<span style="color:blue">**_link_personal_linkedin_**</span> - User's linkedin account URL<br>
<span style="color:blue">**_link_personal_other_**</span> - User's other social media URL<br>
<br>
**_Optional contact phone_**<br>
<span style="color:blue">**_phone1_**</span> - User's phone<br>
<span style="color:blue">**_phone1_verified_**</span> - Weather the user's phone is verified<br>
<span style="color:blue">**_phone2_**</span> - User's additional phone<br>
<span style="color:blue">**_phone2_verified_**</span> - Weather the user's additional phone is verified<br>
<br>

```
account_details
  .account_id
  .avatar_path
  .avatar_shape
  .avatar_shape_radius
  .avatar_updated_at
  .bio
  .city
  .country
  .timezone
  .link_personal_website
  .link_personal_facebook
  .link_personal_xcom
  .link_personal_linkedin
  .link_personal_other
  .phone1
  .phone1_verified
  .phone2
  .phone2_verified
```
<br><br>

### Persistent logins
The `persistent_logins` table is responsible for handling the persistent login tokens, and that - remember me for up to an year checkbox functionality on login.<br>

<span style="color:blue">**_id_**</span> - The id of the record.<br>
<span style="color:blue">**_user_id_**</span> - The id of the user.<br>
<span style="color:blue">**_selector_**</span> - Selector for the persistent login mechanism.<br>
<span style="color:blue">**_token_hash_**</span> - Token hash for the persistent login mechanism.<br>
<span style="color:blue">**_created_at_**</span> - The token creation timestamp.<br>
<span style="color:blue">**_expires_at_**</span> - The token expiration time.<br>
<br>

```
persistent_logins
  .id
  .user_id
  .selector
  .token_hash
  .created_at
  .expires_at
```
<br><br>

### Password resets
The `password_resets` table is responsible for the password resets.<br>

<span style="color:blue">**_email_**</span> - the email address submitted for the password reset.<br>
<span style="color:blue">**_token_**</span> - the password reset token<br>
<br>

```
password_resets
  .email
  .token
```
<br><br>

### Rate limiters
There are a few rate limiters for different account related actions, that we use to hinder the ability of an attacker to brute-force and such.<br>

**_Login Attempts Rate Limiter_**<br>
This functionality limits how many times a user can try to login unsuccessfully before entering a timeout for too many attempts.<br>
<span style="color:blue">**_id_**</span> - The id of the item.<br>
<span style="color:blue">**_email_**</span> - The login email.<br>
<span style="color:blue">**_ip_address_**</span> - The ip address of the user attempting to log in.<br>
<span style="color:blue">**_attempt_time_**</span> - The attempt time?<br>
<br>
**_Register Success Rate Limiter_**<br>
This functionality limits how many accounts can an ip address register.<br>
<span style="color:blue">**_id_**</span> - The id of the item.<br>
<span style="color:blue">**_email_**</span> - The register email.<br>
<span style="color:blue">**_ip_address_**</span> - The ip address of the user registering an account.<br>
<span style="color:blue">**_attempt_time_**</span> - The last registration time?<br>
<br>
**_Password Reset Resend Rate Limiter_**<br>
This functionality limits how many password reset links / emails can a user request.<br>
This serves to limit actors from abusing the forgot password functionality to cause denial of service.<br>
<span style="color:blue">**_id_**</span> - The id of the item.<br>
<span style="color:blue">**_email_**</span> - The user's email.<br>
<span style="color:blue">**_ip_address_**</span> - The ip address of the user requesting a password reset.<br>
<span style="color:blue">**_send_time_**</span> - The timestamp of last reset request?<br>
<br>

```
login_attempts
  .id
  .email
  .ip_address
  .attempt_time

register_success
  .id
  .email
  .ip_address
  .attempt_time

password_reset_resends
  .id
  .email
  .ip_address
  .send_time
```

<br>
<br>

### Links
[Versioning](/listiary/wiki/database/versioning/)<br>
[Subsystems - Main Data](/listiary/wiki/database/main/)<br>
[Subsystems - Metadata (Housekeeping)](/listiary/wiki/database/metadata/)<br>
[Subsystems - Edit history](/listiary/wiki/database/history/)<br>
[Subsystems - Permissions (Authorization)](/listiary/wiki/database/auth/)<br>
<br>
[Listiary Wiki - Database](/listiary/wiki/database/)<br>
[Listiary Wiki - Repo map](/listiary/wiki/repo-map/)<br>
[Back](/listiary/wiki/)
