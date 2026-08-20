wiki for lists,

xxxxx
-------------------------------------------
language for lists - Describe,

xxxxx
-------------------------------------------
monetary policy

I believe that a system should be free and open source, and can still make money in unintrusive ways, which gives it more resilience, than simply waiting for donations.

With listiary, there are few ways. First, admins that host a wiki farm can offer private lists only to paying users, or donors. Then they can offer to host private wikis for paying customers, and, of course, support.Then, donors can also receive stickers, celebrating their support.

Also, on a more controversial note, there might be a market for paid/freemium pluginlets.

Users that are good Listiarians can be hired to write private lists for people, and the platform might make a small percentage, from the person hiring, for providing reputation based marketplace for this work.

Lastly but not least, there is the possibility for paid users on some wikis to lock personally-created unique content for a time, for paid subscribers - like stock market predictions, for example. The key word is for a time window, I imagine from 1 day to one year, after which, the data is released under a foss license.

Of course, the public wiki should always come first.
-------------------------------------------
bot ingested content,

Admins of wikis can run bots that crawl content from reputable sources and create articles on the wiki, designated with low trust raw data level of trust.

I am against AI creating or editing content directly on the platform - I am describing crawling here. 

I dont know what else to say - I mean if there is good data available somewhere, relevant to a knowledge system you are building, and if you can establish a good pipeline - you siphon it in with code - dont just wait for users to eventually add it or not.

Also, this enables the creation of journalling lists, that keep track of something for the users.
-------------------------------------------
client-side federation,

Listiary is built with decentralization, high availability and irregular data sinking upstream or downstream in mind.

A big part of this is the client-side federation model. The way this works is that, a user goes to a Listiary website, or opens the app on his phone, and is able to set secondary databases, to use for pulling data.

Decentralization like that empowers the users, while keeping the system very resilient and diverse.

The client-sidedness leaves different admins free of the responsibility to manage anything besides their own wiki installations. 

For example, if there is a bad wiki - it gets taken down - no great harm is done to Listiary, as opposide to more centralised systems.
-------------------------------------------
Pluginlets
plugins per instance,

the listiary index module supports plugins, and comes with some readily available. Admins can choose wether to enable or disable them, per wiki instance.

Admins can also develop their own plugins. The requirement is that those are written in vanila JS only, and have no dependencies. 
Or rather, it is a guideline some admins might choose to ignore
-------------------------------------------
works as personal tool as well,

People can use listiary for personal use, and we encaurage that. In other words listiary is an encyclopedia and a notebook app in one, and on top of one another.

In listiary, there are 3 kinds of lists - public lists, personal lists, and private lists.

Public lists are the main wiki. People dont generally write public lists, they write personal lists, and propose them to be elevated to public status.

Personal lists can be anything the user wishes to write and share with someone or with the world.

Private lists are for private use. With some wikis, this feature might be available only to donors or paying users.

The idea is simple - with a wiki, you get a better personal knowledge app, and with a personal knowledge app, you get a better wiki, because we get better engagement, and knowledge travels from one to another - from public to personal and private, and helps foster a diverse environment.
-------------------------------------------
content forking,

Listiary adopts the github mentality for lists - every list is forkable. Users also make their own edits, spin multiple versions, etc.

It should be a bit like github for lists.
-------------------------------------------
importable and exportable

Listiary does not try to be the best personal list making app, instead it tries to be a decent one, on top of a knowledge system.

We prioritize interoperability with other apps - export and inport, when possible.
-------------------------------------------
socialmedia shareable

Listiary lists should be easily shareable on social media platforms, like facebook, with one click, and on forums, with some embed codes, and such.

Should be nice and polished.
-------------------------------------------
various levels of trust - liquid trust,

Wikipedia has this dynamic - where if you write an article in a language, you need to cite sources, that there are quite a few of them, that look quite authoritative. Often times, contributors dont do the legwork to dig up and verify the them. 

For example - you want to write an article on a bulgarian dish - all good resources are in bulgarian - so to english speaking moderators, those become a trash-shaped enigma. You can't cite common knowledge as a source either. 

Wikipedia says - be conservative - wikipedia should be unharmed by scandals or inaccurate data.

Listiary says - be everything at once - use federation to protect from scandals - led bad wikis exist and be taken down. Let users write whatever they want, and assign a trust metric to the article, that is ever evolving
-------------------------------------------
plain stack, audit, rewrite and rehost,

I have always been against the paradigm of later years to create software from a whole lot of dependencies. Because it is simply fragile - hard to debug, slow to load and ram hogging, introducing the possibility of various supply chain issues and security vulnerabilities.

Listiary is written in vanilla JavaScript and vanilla PHP, with minimal use of libraries that we host ourselves - one is some css components, other is a JS cryptographic function implementation.

A wiki engine dos not need to implement features fast to compete, or vast complexity - it needs stability, security and maintainability.

My policy is - if we shall use a library, we find a FOSS one, we audit a version, and host it ourselves. But, if we can do that, why not rewrite the parts that we need. So that is - rewrite or audit and self-host - dont use premade functionality that is more elaborate than it should be, comes bundled in a bigger library, por locks us in some architecture.
-------------------------------------------
data written from the inside out

Like other wikis ang knowledge systems that organically grow, Listiary is developed with the idea that the contained information will ever shift and change names and places.

Listiary is then like the data - modular, extentible, and evolving.
-------------------------------------------
facing outwards - index of the web

Listiary is not a self-contained knowledge system - it is a structure of knowledge, and many items in the lists have links outside tge site.

Think of it not as an encyclopedia, but as an index of the internet and human knowledge on a given topic.
-------------------------------------------
FOSS

Both Listiary and Describe are Free and Open Source, licensed under AGPL v3. In fact, they are copy-lefted - meaning users cannot build proprietary software on top of the components.

Admins however, can host Listiary instances and profit from them by the freemium model - by offering paid services, such as private wiki hosting, support, and such.
-------------------------------------------
online-offline sinc high availability model

Many web apps today are built with the basic premise that you will simply have internet. And if you dont, you cant use the app. 

Listiary is built with decentralization, high availability and irregular data sinking upstream or downstream in mind.

The reason is twofold - for one, we want to give the user the basic right to controll where the data comes from vs where the app talks to.

for another - from a wiki knowledge system we want resilience, that serves the user best and can survive splinternet, a nuclear halaucost and a cyborg uprising - not a service that dissapears the first time there is a google or aws outage, or turns commercial when the CEO of a service changes.

basically, I believe a user should be in controll of what gets pulled locally, and what is synced from and to, and when - if he wants to, and not be bothered if he does not.