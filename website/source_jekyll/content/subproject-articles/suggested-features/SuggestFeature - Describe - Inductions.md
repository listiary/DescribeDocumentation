---
layout: page
title: SuggestFeature - Describe - Inductions
permalink: /listiary/articles/qjgeali6kw/
exclude: true
---
<br>
```
Article type: Feature Suggestion
Article name: SuggestFeature - Describe - Inductions
Affected Software/module: Describe Language
Author:	Framez
```
<br><br>

## Description:
The idea is that we have regular lists, that we can also call productions - they have a production arrow - `->`.
So why not have induction lists, called also inductions - with an induction arrow - `<-`.
The symbols for the arrow are similar, so it will be easy to implement in the Describe grammar.
<br><br>
The whole idea is that, if we want to have this compound items - that are lists on their own,
full of items that are decorators, strictly speaking, so they don't need tilde inversions at all - 
they are just all decorators.
<br><br>

### Regular list:
```
my car ->

	~ yellow <color>,
	~ Opel Corsa <brand>,
	~ induction arrow demo <context>;
```

### Induction list:
```
my car <-

	yellow <color>,
	Opel Corsa <brand>,
	induction arrow demo <context>;
```
<br><br>

### Original draft example text (induction, colon notation):
```
my car <-

    color: yellow,
    brand : Opel Corsa,
    context: induction arrow demo;
```

<br><br>
### Links
[Back](/listiary/articles/)<br>