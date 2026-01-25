---
layout: page
title: Listiary Wiki - Repo map
permalink: /listiary/wiki/repo-map/
exclude: true
---
<br>
In the repository for the Listiary wiki project, we have a few special folders, like `.work`, `.media`, `.documentation` - e.g., and many more functional ones - each containing a module of the web app. In this article we will describe the folders layout in some detail. Also, The layout in the work folder is a bit messy and will evolve over time.
<br><br>

### 1. Documentation

`/.documentation`

In the documentation folder we store all the local documentation - like bug reports, change logs for different modules, etc. You might ask - why not store the documentation in the DescribeDocumentation repo - and we do eventually copy some of this local documentation there, and turn it to articles. But this is the local place for storing all kinds of documentation drafts and such.
<br>
<br>

### 2. Media

`/.media`

In the media folder we store all kinds of images, related to the projects. Those are mostly various icons used in the website.
<br>
<br>

### 3. Work

`/.work`

In the work folder we do actual development. Here, we have old versions of stuff - like this module or the whole website, and we have folders that contain small sub-projects. The ones that are purely archival are in folders that start with a dot - '.Old Listiary Versions', '.Old Listiary Versions - Last', '.Minified' - containing copies of minified scripts - etc. and the others - well - does not. Here is a list:

`/.Old Listiary Versions`<br>
Archive of different versions of the Listiary web app.<br>
<br>
`/.Old Listiary Versions - Last`<br>
Last version of the Listiary web app - to be used to copy codes from.<br>
<br>
`/.Minified`<br>
Archive of our scripts that we have minified.<br>
<br>
`/index-tools`<br>
Contains individual tools into individual '.js' files. We eventually concatenate those into one script for better loading - 'listiaring.js'. We have a "/.not-used" folder which contains scraped tools' drafts.<br>
<br>
`/.index-scripts`<br>
Archive of the index module main scripts - both for the mobile and for the full versions.<br>
<br>
`/.index-plugins`<br>
Work directory and archive for the plugins for the Listiary web app.<br>
<br>
`/.index-main-tree`<br>
Archive for the main tree library we are developing.<br>
<br>
`/.index-listiaring`<br>
Archive for the 'listiaring.js' files versions we built from our tools in the past.
<br>
<br>

### 4. Modules

`/sources`<br>
Sources - Local sources / payloads for testing with the local files plugin.<br>
<br>
`/session`<br>
Session - The session module for the web app.<br>
<br>
`/search`<br>
Search - This folder is empty yet, but it will contain the search module, which has not been developed yet.<br>
<br>
`/index`, `index.php`, `favicon.ico`<br>
Index - The index module - the full version of the site.<br>
<br>
`/m.index`, `m.index.php`, `favicon.ico`<br>
Mobile Index - The mobile index module - the full version of the site.<br>
<br>
`/editor`<br>
Editor - The editor module (Using Codemirror. Not great. Should try Monaco)<br>
<br>
`/docs`<br>
Documentation pages - like terms of service, licensing, and cookie consent documents.<br>
<br>
`/contact`<br>
Contact pages mobile and full.
<br>
<br>

### Links
[Listiary Wiki](/listiary/wiki/)<br>
[Listiary Wiki - Plugins](/listiary/wiki/plugins/)<br>
[Listiary Wiki - Index](/listiary/wiki/index/)<br>
[Listiary Wiki - Scripts](/listiary/wiki/scripts/)<br>
<br>
[Back](/listiary/)
