Article type: 						`Suggest Feature`<br>
Article name:						`SuggestFeature - Describe - Compound headings`<br>
Affected Software/module:			`Describe Language`<br>
Author:								`Framez`<br>

## Description:
The idea that a list entry can be made of few parts of data, and we should
have some interface - like in the menu, to shift and filter those, is a cornerstone
of Listiary magic - it is a part of the interactivity - of why, this wiki with the 
specific markup language for lists is better at representing lists than a regular wiki engine.

This has not been implemented yet, but we can do this, and we will.

The way I imagine this, is with using items structurally. I think of retiring tildes in favor of something
simpler, like a colon. But either way, a tilde, or a colon notation, is a way of representing items in a 
list like decorators. For example, let's look at a title of a song as a regular item:

```
Mike Oldfield - Moonlight Shadow ft. Maggie Reilly
```

Then, with a tilde notation, it becomes:

```
(artist) - (title) ft. (artist1) ->

    ~ Mike Oldfield <artist>,
	~ Moonlight Shadow <title>,
	~ Maggie Reilly <artist1>;
```

In colon notation, it becomes:

```
(artist) - (title) ft. (artist1) ->

    :artist Mike Oldfield,
	:title Moonlight Shadow,
	:artist1 Maggie Reilly;
```

This is introducing OOP to describe, and I am debating about the colon notation,
and not sure what kind of brackets to use. Still not implemented in the language,
but should be upcoming in the next major version.

The original remark:
```
Artist - Song VS Song - Artist on mobile for better readability
```