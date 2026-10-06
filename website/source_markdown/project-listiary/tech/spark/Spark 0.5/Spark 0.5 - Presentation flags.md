---
layout: page
title: Spark v0.5 - Presentation flags
permalink: /listiary/wiki/spark/v05/flags/
exclude: true
---
<br>
In this article we will look at flags for altering the presentation of the output, and default behavior.
<br><br>

The presentation flags are a number of flags and values that changes the way Spark CLI outputs data.
They are used for user convenience and for fine-tuning the tool - for example for execution manually vs in automated scripts.
<br><br>

_**flag:**_ `auto`<br>
Removes the colors, for use in scripting.
In PHP CLI, the console colors are special command characters that we output to change the color.
This flags stops this behavior, so that no color command characters are outputted.<br>
_syntax (all are valid):_ `auto`, `a`, `-a`, `-auto`, `--auto`
<br><br>

_**flag:**_ `hide-banner`<br>
Removes the ASCII art banner, for use in scripting.<br>
_syntax (all are valid):_ `hide-banner`, `hb`, `-hidebanner`, `-hb`, `--hide-banner`
<br><br>

_**flag:**_ `theme=`<br>
Sets the color theme of the CLI text output.<br>
_syntax:_ `theme=<THEME>`<br>
_THEME:_ `GREEN`, `DBLUE`, `LBLUE`, `PASTEL`, `EARTH`, `CONTRAST`, `DEFAULT`, `VIOLET`, `CYAN`
<br><br>


### Links
[Back](/listiary/wiki/spark/v05/)