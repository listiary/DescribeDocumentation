---
layout: page
title: Listiary Wiki - Scripts
permalink: /listiary/wiki/scripts/
exclude: true
---
<br>
The Listiary wiki is JavaScript and PHP based - and it has a lot of vanilla JavaScript. So much so, that it has became hard to manage - we struggle with integrating new functionality - at least I do - to figure out what function was used for what, how to extend a class properly, and how not to break existing code, etc. And this is an issue that both arises in software development with some regularity, and needs to be fixed when it does - such is the development cycle. But in this case, we have hit another wall - plain JavaScript is simply ill suited for larger projects. This is why we will be transitioning to Type Script - which will bring structure and strong typing, and still produce the vanilla JavaScript we hope to preserve.

My point is - no need to write detailed documentation for a codebase we will be restructuring anyway. But we will give some explanation at which script file does what, in this article.
<br><br>

### 1. Mobile Index

`/m.index/js/scripts.options.js`<br>
`/m.index/js/plugin.base.js`<br>
`/m.index/js/plugin.stream-player.js`<br>
`/m.index/js/plugin.local-loader.js`<br>
`/sources/payload.js`<br>
<br>
`/m.index/js/listiaring.tool-management.js`<br>
`/m.index/js/listiaring.tooling.js`<br>
`/m.index/js/listiaring.common.js`<br>
`/m.index/js/listiaring.common-tools.js`<br>
`/m.index/js/listiaring.js`<br>
<br>
`/m.index/js/mobile-detector.js`<br>
`/m.index/js/main-tree.js`<br>
`/m.index/js/crypto-js.min.js`<br>
<br>
`/m.index/js/scripts.more.js`<br>
`/m.index/js/scripts.dom-manipulate.js`<br>
`/m.index/js/scripts.dom-create.js`<br>
`/m.index/js/scripts.redirects.js`<br>
`/m.index/js/scripts.crypto.js`<br>
`/m.index/js/scripts.json-loader.js`<br>
`/m.index/js/scripts.js`<br>
<br>
<br>

### 1.A. Options
`scripts.options.js`<br>
<br>
Contains all the options for Listiary, most of which users can set - like color themes and such.
<br>
<br>

### 1.B. Plugins
`plugin.base.js`<br>
`plugin.local-loader.js`<br>
`plugin.stream-player.js`<br>
<br>
This is the plugin functionality. The plugin.base contains the `ListiaryPlugin` base class, that all the plugins extend, and the other are simply plugins, already implemented. For more info on plugins, read [Wiki - Plugins](/listiary/wiki/plugins/).
<br>
<br>

### 1.C. Local Payload
`/sources/payload.js`<br>
<br>
A test payload that can be loaded with the Local Loader plug in, in order to develop the front end without a database.
<br>
<br>

### 1.D. Tooling
`listiaring.tool-management.js`<br>
`listiaring.tooling.js`<br>
`listiaring.common.js`<br>
`listiaring.common-tools.js`<br>
`listiaring.js`<br>
<br>
`listiaring.tooling.js` contains the base classes for all the tools, and `listiaring.tool-management.js` contains the tool tracker and manager, used to track tool usage history, set / unset trigger groups, and create new list variants as tools are selected.
`listiaring.common.js` contains functions used in tool making - like `_createTriggerElement` or `_addAfter` that create or add trigger elements to a sub-menu, and `listiaring.js` is where the actual tools' instances are declared and initiated (added to the menus) - in other words - this is where the actual tools live.
<br>
<br>

### 1.E. Mobile Detector
`mobile-detector.js`<br>
<br>
This is a class that detects the type of media we run on - so that if it is `small` or `mobile`, we can show the mobile version of the site.
<br>
<br>

### 1.F. Main Tree
`main-tree.js`<br>
<br>
The tree view we are using. It comes from a free and open source (FOSS) library we have modified addopted to our needs.
It is of significant importance to the project, to be able to visualize the trees, so this is a big one.
<br>
<br>

### 1.G. Crypto
`crypto-js.min.js`<br>
`scripts.crypto.js`<br>
<br>
This one provides encryption in a way that is compatible with our PHP and C# implementations.
It is crucial for private lists' end to end encryption, as they need to be decrypted in the browser - which is what `scripts.crypto.js` does.
It is a third party library, available here (crypto-js v4.0.0)[https://cdnjs.com/libraries/crypto-js/4.0.0].
<br>
<br>

### 1.H. Main Scripts
`/m.index/js/scripts.more.js`<br>
`/m.index/js/scripts.dom-manipulate.js`<br>
`/m.index/js/scripts.dom-create.js`<br>
`/m.index/js/scripts.redirects.js`<br>
`/m.index/js/scripts.crypto.js`<br>
`/m.index/js/scripts.json-loader.js`<br>
`/m.index/js/scripts.js`<br>
<br>
The main scripts for the app. `dom-create` and `dom-manipulate` are responsible for DOM interactions, `crypto` provides an in-browser decryption capability, `redirects` contain all the redirect functions, `json-loader` loads JSON payloads into the app, and `scripts.js` is the main script - where the main sequence is done - the initial loading of the JSON payload. It is the kind of unofficial 'entry point' for the app scripts.
<br>
<br>

### Links
[Listiary Wiki](/listiary/wiki/)<br>
[Listiary Wiki - Repo map](/listiary/wiki/repo-map/)<br>
[Listiary Wiki - Plugins](/listiary/wiki/plugins/)<br>
[Listiary Wiki - Index](/listiary/wiki/index/)<br>
<br>
[Back](/listiary/)
