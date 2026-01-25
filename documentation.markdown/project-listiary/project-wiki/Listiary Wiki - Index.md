---
layout: page
title: Listiary Wiki - Index
permalink: /listiary/wiki/index/
exclude: true
---
<br>
The listiary wiki is a php/javascript based software, consisting of few modules. Each module has its own folder that contain all the files, except for the Index module - where the main php files are outside the module folder, into the main directory - as they are the main pages of the web app. Let's see what the index does.
<br><br>
`/index`<br>
`index.php`<br>
`/m.index`<br>
`m.index.php`<br>
`favicon.ico`<br>
<br>
These are the main pages of the Listiary web app - `m.index.html` and `index.html` - the mobile and the desktop version, and the favicon for the app/site - `favicon.ico`. All other files in the module are contained inside the `/index` and `/m.index` folders - media, css, javascript files, etc. The mobile version is the one being developed at the moment, and we will dissect it, for this reason.
<br>
<br>
In the head, we have a reference to the main CSS for the page - `/index/m.index.styles.css`.
And in the body, we have:
- The sidenav section - that is the content inside the hamburger menu.
- The triggers section - currently has only one trigger - that hamburger button for the menu.
- The main page skeleton table.
- The scripts section - where all the scripts for the module are loaded.
<br>
<br>

### 1. Scripts
Apart from the CSS, the website index functionality resides in the JavaScript files.
Look at [Listiary Wiki - Scripts](/listiary/wiki/scripts/) for more on scripts.
<br>
<br>

### 2. Triggers
Triggers are those icons on the website header. At the moment we have only one trigger - that hamburger button - that opens the side navigation menu. But we will probably, at least add a search button in the future. We also had the idea of having a language button - where you can choose from different language versions of the current list - just like on wikipedia.
<br>
Pressing the hamburger button calls `openNav()` from the main script - making the sidenav visible.
<br>
<br>

### 3. Sidenav
First, we have the close button inside the sidenav - that closes the sidenav by calling `closeNav()` from the main script - making the sidenav invisible. Then, we have the "show next menu" arrow - that shows the menu with all the tools, by calling `showNextMenu()`. The rest is the main menu, and the next menu - with the tools. From that menu with the tools, we have a submenu for each tool category. It opens a specific sub-menu by hiding/unhiding elements. Those menus contain 3 anchor elements each - the first is a new line element, and the other two are horizontal lines - `hr`. All the tools are added as plugin scripts, and they add their elements (triggers) in those sub-menus. And here is what those sub-menus are about:

- Highlighters - tools that you choose to highlight elements in different colors - in a highlighter fashion.
- Sorters - tools that sort the list - alphabetically, by some decorator, etc.
- Copiers - tools that copy elements being clicked - the text, copy as Json, etc.
- Pickers - tools to pick a random element.
- Viewers - tools to hide or show different pieces of data in the entries.
- Filters - tools to filter entries.
- Languages - Toggle different language versions of the list, if any other languages are available.
- Plugins - The Listiary plugins.
- Droppers - The idea of having droppers, however useful or not, is this - like we have pickers that pick a random entry, by some criteria, droppers will remove a random entry from a list, by some criteria.
- Extenders - The idea of having extenders, is this -
<br>
<br>

### 4. Main scaffolding / page skeleton
We use a table for organizing the page layout. Nothing special here.
The mobile version has 2 rows / cells - the top container and the main container.
The main container also contains the bottom toolbar - those circular controls on longer lists.
<br>
<br>

### Links
[Listiary Wiki](/listiary/wiki/)<br>
[Listiary Wiki - Repo map](/listiary/wiki/repo-map/)<br>
[Listiary Wiki - Plugins](/listiary/wiki/plugins/)<br>
[Listiary Wiki - Scripts](/listiary/wiki/scripts/)<br>
<br>
[Back](/listiary/)
