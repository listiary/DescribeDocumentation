Listiary is a wiki built from nested lists on various topics. From movie recommendations and playlists to knowledge maps and personal journals.
It’s a flexible, open-source tool for building structured wikis of lists on any topic.


Listiary is an experimental wiki project built around lists rather than articles. The basic idea is simple: lists are treated as their own kind of object, not as formatting inside text. That decision shapes most of the system, from how content is written to how it changes over time.



## About  
Apart from being a free and open source wiki engine, built around nested lists, Listiary embodies quite a few design choices, that are unusual for wiki platforms. And this is intentional, because we are experimenting with them, to see which ones do great, in our platform. Below are the most prominent ones.

Core ones:
***Language for Lists*** - Listiary has its own small language for writing lists, called Describe. It’s meant to be readable and consistent, without feeling like programming. (OLD: Describe is intuitive – anyone can write in it without formal trainig, allowing rich, interactive lists to be created by anyone.)

***Plain tech stack*** - Listiary is written in vanilla JavaScript and vanilla PHP, with minimal use of libraries that we host ourselves, so it is secure, lightweight and easy to audit. (OLD: Listiary is a custom platform implemented in plain JavaScript and PHP, without dependencies that could introduce vulnerabilities or maintenance overhead.)

***FOSS*** - Both Listiary and Describe are Free and Open Source, licensed under AGPL v3.

Experimental ones:

***Personal tool*** - People can use Listiary for personal use, and we encourage that. In other words, Listiary is an encyclopedia and a notebook app in one, and on top of one another.

***Extensdible*** - Listiary supports plugins, and comes with some readily available. Admins can choose whether to enable or disable them, per wiki instance. Admins can also develop their own plugins. (OLD: Developers can write and submit their own add-ons, and users can enable different add-ons to customize their experience. Think music players, fonts and styles, etc.)

***Bot-derived content*** - Admins of wikis can run bots that crawl content from reputable sources and create articles on the wiki, designated with a low-trust system resilience to match (REWRITE LAST PHRASE).

***Distributed and sustainable*** – Users choose servers and content to load, giving Listiary a decentralized model. Listiary is built with decentralization, high availability, and irregular data syncing upstream and downstream in mind. A big part of this is the client-side federation model. This flexibility makes a huge difference in terms of moderation and long-term sustainability, compared to rigid centralized platforms.

***Interactive editing*** – Users can customize, edit, highlight, and sort public or personal lists, with versioned drafts saved for later, fork their own versions, and even share them on social media if they like.

***Inportable and Exportable*** - Listiary does not try to be the best personal list-making app. Instead, it tries to be a decent one on top of a knowledge system. We prioritize interoperability with other apps: export and import whenever possible.

***Forkable content*** - Listiary adopts the GitHub mentality for lists: every list is forkable. Users can make their own edits, maintain multiple versions, and let different versions evolve independently.

***liquid trust*** - Flexible layered trust model. Let users write whatever they want, and assign an ever-evolving trust metric to the article.

