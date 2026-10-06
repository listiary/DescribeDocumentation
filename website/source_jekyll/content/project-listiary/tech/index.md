---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults

layout: page
title: Listiary Technical Reference
permalink: /listiary/wiki/tech/
exclude: true
---
<br>
This is the technical reference for the Listiary wiki platform.

Describe is built and developed for Listiary, but can also be used on its own. Both Listiary and Describe are free and copyleft-ed, under the [GNU Affero General Public License, version 3 (AGPLv3)](https://www.gnu.org/licenses/agpl-3.0.html).

Here you can find documentation on the architecture, components, modules, infrastructure, and other technical aspects of Listiary and its supporting software.
This section is currently under development.
<br><br><br>


### Modules of Listiary
<img src="{{ site.baseurl }}/assets/images/listiary-modules-2.png" alt="listiary-modules" style="height:auto; width:auto; max-width:100%; max-height:320px;">
<br><br>

The Listiary system can be divided into four layers:
- hosting infrastructure
- administrative modules
- user-facing modules
- standalone pages
<br><br>

Hosting Layer - A Listiary installation requires conventional PHP/SQL-capable web hosting and an Amazon Web Services (AWS) account for its server-side services - namely the Describe compiler. The documentation site is hosted separately as a static site and does not need to be hosted by individual Listiary administrators.
- PHP capable web hosting
- SQL server (Maria DB compatible)
- AWS lambda function micro service
- Hosting for the static documentation site
<br><br>

Administrative Modules - The administrative layer provides the tools required to install, configure, and administer a Listiary instance. It also includes the Session Module, which manages access and permissions, and Spark CLI, a separate console application for administering a Listiary backend from an operating-system console.
- `Web Installer` - PHP based installer/configurator
- `Web Admin` - The admin panel
- `Session Module` - The accounts and session management
- `Spark CLI` - OS based admin framework. Separate software
<br><br>

Userland Modules - These are the modules that users interact with during normal use of Listiary.
- `Index Module` - the usual wiki view
- `Editor Module` - the Describe editor
- `Code Viewer Module` - similar to the editor, but read-only
- `History Module` - view/compare edit history
- `Search Module` - the search page/engine
<br><br>

Standalone Pages - These are standalone pages that are adjacent to the core Listiary system and do not need to interact with it at a deeper level. The documentation site and legal pages are examples: they are part of the overall Listiary project, but do not depend on the wiki functionality itself.
- `Documentation` - This documentation website
- `Legal Docs` - ToS, Cookie Consent, Privacy Policy and such
- `Contact Us` - contact us / bug report forms
<br><br><br>


### Modules
[Listiary Wiki - Spark](/listiary/wiki/spark/)<br>
[Listiary Wiki - Database](/listiary/wiki/database/)<br>
<br><br>

### Links
[User Documentation](/listiary/wiki/user/)<br>
[Site SubMap](/listiary/maps/submap-listiary/)<br>
<br>
[Back](/listiary/)<br>
