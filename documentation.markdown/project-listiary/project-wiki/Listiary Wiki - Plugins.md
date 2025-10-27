---
layout: page
title: Listiary Wiki - Plugins
permalink: /listiary/wiki/plugins/
exclude: true
---
<br>
The Listiary Wiki relies quite extensively on plugins to add functionality to the minimalist core app. This design offers several advantages - like modularity, extensibility, and the ability to gradually open-source parts of the codebase. In this article, we’ll explore the built-in plugins that ship with the wiki and examine the roles they play.
<br><br>

### 1. Local Loader
The Local Loader is a plugin intended for debugging purposes - it is not intended for production code.
It is used to bypass the PHP source loading sequence and load a local JS / JSON file instead - from the website's `sources` folder.
<br>
<br>

### 2. Stream Player
The Stream Player plugin is an audio player with a visualization, that plays audio streams directly inside Listiary.
The way this works is by reading the contents of a list before it is being visualized and determining wether it contains playable audio streams. If so, the player is displayed, and those items containing the streams are highlighted with a particular color, and their behaviour is altered, so that they no longer open a link in new tab, but instead change the source stream of the stream player.
It has 3 modes of operation - TestMode, ExtensionMode and DecoratorMode. In extension mode, the plugin will scan all the items' last links (if more than one) for an extension that is known to be an audio stream. In decorator mode, the player will scan items for decorators `audio-stream` or `radio-stream`, and in test mode, the player will appear inside a list with a given id, and will play a predetermined audio source when played - regardless of the list's contents - just for the sake of testing the player - but this last option will be removed for production.
<br>
<br>

### 3. Youtube Player
The Youtube Player plugin is similar to the Stream Player plugin - only it will play a youtube video directly inside Listiary.
It has not been implemented yet.
<br>
<br>

### 4. Soundcloud Player
The Soundcloud Player plugin is similar to the Stream Player plugin - only it will play a youtube video directly inside Listiary.
It has not been implemented yet.
<br>
<br>

### 5. Modal Shower
The Modal Shower is a plugin that shows different full-screen messages on top of the other content - aka. modal forms.
The plugin has not been implemented yet.
<br>
<br>

### 6. Stat Viewer
The Stat Viewer plugin will show statistical data about an entry - how many entries it contains, how many links, etc.
The plugin has not been implemented yet.
<br>
<br>

### 7. App Tutor
The App Tutor will be an UX tour of the app - the kind with "click here to do that" messages.
The plugin has not been implemented yet.
<br>
<br>

### Links
[Listiary Wiki](/listiary/wiki/)<br>
[Listiary Wiki - Repo map](/listiary/wiki/repo-map/)<br>
[Listiary Wiki - Index](/listiary/wiki/index/)<br>
[Listiary Wiki - Scripts](/listiary/wiki/scripts/)<br>
<br>
[Project Listiary](/listiary/)<br>
[Project Describe](/language/)
