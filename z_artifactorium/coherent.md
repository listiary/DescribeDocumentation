If I were an intelligent developer encountering Listiary for the first time, what impression would these documents give me?

You want to know whether the collection communicates:

“This person has thought deeply about this.”
“This is an unusual but coherent project.”
“I understand what Listiary is trying to accomplish.”
“There are interesting technical ideas here.”
“I want to see where this goes.”

versus:

“This is grandiose.”
“This person is inventing terminology for things that already exist.”
“I don't understand what problem this solves.”
“The author seems dogmatic.”
“The architecture sounds clever but I don't know what it actually does.”
“This is a personal manifesto rather than useful documentation.”

Clarity - Can a technically competent stranger understand the idea?
Credibility - Does the author sound like they know what they're doing?
Coherence - Do the 20 pieces form a recognizable philosophy/system?
Intrigue - Does this make someone want to learn more?
Practicality - Can I understand what Listiary actually does?
Tone - Confident, uncertain, dogmatic, grandiose, pragmatic?
Originality - Are there genuinely interesting ideas here?
Documentation value - Would this help a prospective user/developer?
Red flags - What makes the project look confused or unrealistic?
Voice- Does the author's personality help or hurt the project?

```
## Project Homepage

Listiary is an experimental wiki project built around lists rather than articles. The basic idea is simple: lists are treated as their own kind of object, not as formatting inside text. That decision shapes most of the system, from how content is written to how it changes over time.


Instead of assuming a single central wiki, Listiary uses a distributed model. Content can live on different servers, and people choose which sources they want to load or follow. There’s no requirement that everything collapse into one canonical version, which makes it easier for lists to diverge, evolve, or exist in parallel.


Listiary also has its own small language for writing lists, called Describe. It’s meant to be readable and consistent, without feeling like programming. The language exists mainly to make lists easier to express, compare, and process, not to be clever for its own sake.


The platform is intentionally built in a straightforward way, using plain JavaScript and PHP. The goal is to keep the system understandable and maintainable over time, rather than optimized for scale or growth. It’s closer to something you can read and tinker with than something you have to learn around.


This is still a work in progress. We’re developing it carefully, because the ideas feel interesting enough to explore properly. There’s no fixed roadmap or end state in mind; we’re building it, paying attention to how it behaves, and seeing where it leads.
_____________________________________________________________________________________________________________________________________

## Axiome - Wiki for Lists

Listiary is an wiki software built around lists rather than articles. The basic idea is simple: lists are treated as their own kind of object, not as formatting inside text.

This, paired with the markup language we have invented, and some of the other experimental features, makes it a more powerful and flexible system for lists than standard wikis, and something of a test-bed for some design choices on a wiki platform.

I would summarize it as - wiki platform that is decentralized and resilient like Mastodon, and agile with lists like - well, a decent software for lists, with some novel architectural and design choices on top.
_____________________________________________________________________________________________________________________________________

## Axiome - Language for Lists

Listiary has its own small language for writing lists, called Describe. It’s meant to be readable and consistent, without feeling like programming. What WikiMarkup is to Wikipedia, Describe markup is to Listiary.

Describe is a domain specific markup language designed to write and maintain complex data lists that are compiled on demand to various formats, such as HTML, XML, SQL and JSON. It is simple to use, intuitive and easy to master. Describe is readily extendable - implementing support for new target languages or customizing the transpilation process is straightforward, making it adaptable to a wide range of projects.

It is a standalone language as well - perfectly usable on its own. In the Listiary ecosystem, it is used to transpile Describe Markup to JSON - that JSON is used in the wiki engine.
_____________________________________________________________________________________________________________________________________

## Axiome - Free and Open Source

Both Listiary and Describe are Free and Open Source, licensed under AGPL v3. In fact, they are copylefted, meaning that modified and derivative versions cannot simply be turned into proprietary software.

Admins, however, can host Listiary instances and profit from them through a freemium model, by offering paid services such as private wiki hosting, support, and such services.
_____________________________________________________________________________________________________________________________________

## Axiome - Plain Software Stack

`plain stack, audit, rewrite and rehost`

I have always been against the paradigm of recent years to create software from a whole lot of dependencies. It is simply fragile: hard to debug, slow to load, RAM-hogging, and introducing the possibility of various supply-chain issues and security vulnerabilities.

Listiary is written in vanilla JavaScript and vanilla PHP, with minimal use of libraries that we host ourselves. One is some CSS components, another is a JavaScript cryptographic function implementation.

A wiki engine does not need to implement features fast to compete, or have vast complexity. It needs stability, security, and maintainability.

My policy is: if we shall use a library, we find a FOSS one, audit a version, and host it ourselves. But if we can do that, why not rewrite the parts that we need?

So that is the policy: rewrite, or audit, and self-host. Don’t use premade functionality that is more elaborate than it should be, comes bundled in a bigger library, or locks us into some architecture.
_____________________________________________________________________________________________________________________________________

## Experimental - Personal Tool

People can use Listiary for personal use, and we encourage that. In other words, Listiary is an encyclopedia and a notebook app in one, and on top of one another.

In Listiary, there are three kinds of lists: public lists, personal lists, and private lists.

Public lists are the main wiki. People don’t generally write public lists directly. They write personal lists and propose them to be elevated to public status.

Personal lists can be anything the user wishes to write and share with someone or with the world.

Private lists are for private use. With some wikis, this feature might be available only to donors or paying users.

The idea is simple: with a wiki, you get a better personal knowledge app, and with a personal knowledge app, you get a better wiki. We get better engagement, and knowledge travels from one to another, from public to personal and private, and back again, helping foster a diverse environment.
_____________________________________________________________________________________________________________________________________

## Experimental - Pluginlets

`Pluginlets - plugins per instance`

The Listiary index module supports plugins, and comes with some readily available. Admins can choose whether to enable or disable them, per wiki instance.

Admins can also develop their own plugins. The requirement is that those are written in vanilla JS only, and have no dependencies. Or rather, it is a guideline some admins might choose to ignore in the future.

But, I see the pluginlets as small, 1 file apps written in plain JS, that interact with the data in the loaded article to figure out if they should run in that page, and if so, they modify the content in some way, or add a control on top of the list, for example.
_____________________________________________________________________________________________________________________________________

## Experimental - Bot-ingested Content

Admins of wikis can run bots that crawl content from reputable sources and create articles on the wiki, designated with a low-trust, raw-data level of trust.

I am against AI creating or editing content directly on the platform. I am describing crawling here.

I mean, if there is good data available somewhere, relevant to a knowledge system you are building, and if you can establish a good pipeline, you siphon it in with code. Don’t just wait for users to eventually add it or not.

This also enables the creation of journaling lists that keep track of something for the users.
_____________________________________________________________________________________________________________________________________

## Experimental - Client-side Federation

Listiary is built with decentralization, high availability, and irregular data syncing upstream and downstream in mind.

A big part of this is the client-side federation model. The way this works is that a user goes to a Listiary website, or opens the app on their phone, and is able to set secondary databases to use for pulling data.

Decentralization like that empowers the users while keeping the system resilient and diverse.

The client-side nature leaves admins free of the responsibility to manage anything besides their own wiki installations.
_____________________________________________________________________________________________________________________________________

## Experimental - Flexible Sync Model

`online-offline flexible sync, high availability model`

Many web apps today are built with the basic premise that you will simply have internet. And if you don’t, you can’t use the app.

Listiary is built with decentralization, high availability, and irregular data syncing upstream or downstream in mind.

The reason is twofold. For one, we want to give the user the basic right to control where the data comes from vs. where the app talks to.

For another, as a wiki knowledge system, we want a decentralized system with baked-in resilience that serves the user best and can survive splinter-net, a nuclear holocaust, and a cyborg uprising, not a service that disappears the first time there is a Google or AWS outage, or changes its terms when the people running it change their mind.

Basically, I believe a user should be in control of what gets pulled locally, what gets synced, where it gets synced to, and when, if they want to. And they shouldn’t be bothered by it if they don’t.
_____________________________________________________________________________________________________________________________________

## Experimental - Importable and Exportable

Listiary does not try to be the best personal list-making app. Instead, it tries to be a decent one on top of a knowledge system.

We prioritize interoperability with other apps: export and import whenever possible.
_____________________________________________________________________________________________________________________________________

## Experimental - Content Forking

Listiary adopts the GitHub mentality for lists: every list is forkable. Users can make their own edits, maintain multiple versions, and let different versions evolve independently.

It should be a bit like GitHub for lists.
_____________________________________________________________________________________________________________________________________

## Experimental - Liquid Trust

`various levels of trust - liquid trust`

Wikipedia has this dynamic where, if you write an article in a language, you need to cite sources, and there needs to be quite a few of them, that look quite authoritative. Often, contributors don’t do the legwork to dig them up and verify them, not because they are simply lazy, but often because it costs money to buy the actual books or research-articles.

For example - You want to write an article about a Bulgarian dish. All the good resources are in Bulgarian, so to English-speaking moderators, those resources become a trash-shaped enigma - no one will track them, buy them, and get them professionally translated. You can’t cite common knowledge as a source either. You can cite a menu in English - that only serves as a final proof of your correctness to you - but to moderators - they don’t see that.

In other words, Wikipedia says: be conservative. Wikipedia should be unharmed by scandals. Wikipedia should strive for maximum data accuracy, even if this means omitting a lot of knowledge. Listiary says: be everything at once. Use federation to protect from scandals - let bad wikis exist and be taken down. Let users write whatever they want, and assign an ever-evolving trust metric to the article.


P.S. This is not to say that Wikipedia is wrong - they have a different model of doing things, that fits them being this pillar of knowledge. Then, in a world with Wikipedia, we might implement other models.
_____________________________________________________________________________________________________________________________________

## Remark - Facing Outwards

`facing outwards - index of the web`

Listiary is not a self-contained knowledge system. It is a structure for organizing knowledge, and many items in the lists have links outside the site.

Think of it not as an encyclopedia, but as an index of the internet and human knowledge on a given topic.
_____________________________________________________________________________________________________________________________________

## Remark - Inside Out

`data written from the inside out`

Like other wikis and knowledge systems that organically grow, Listiary is developed with the idea that the contained information will constantly shift, change, and move around.

Listiary is then like the data itself: modular, extensible, and evolving.
_____________________________________________________________________________________________________________________________________

## Remark - Social Media Shareable

Listiary lists should be easily shareable on social media platforms, like Facebook, with one click, and on forums with embed codes and such.

They should be nice and polished when shared, too.
_____________________________________________________________________________________________________________________________________

## Remark - Monetary Policy

I believe that a system should be free and open source, and can still make money in unobtrusive ways. This gives it more resilience than simply waiting for donations.

With Listiary, there are a few ways.

First, admins that host a wiki farm can offer private lists only to paying users or donors.

Then they can offer to host private wikis for paying customers, and, of course, support.

Donors can also receive stickers celebrating their support.

Also, on a more controversial note, there might be a market for paid/freemium pluginlets.

Users that are good Listiarians can be hired to write private lists for people, and the platform might make a small percentage from the person hiring, for providing a reputation-based marketplace for this work.

Lastly, but not least, there is the possibility for paid users on some wikis to lock personally-created unique content for a time, for paid subscribers, like stock market predictions, for example. The key word is for a time window. I imagine anything from one day to one year, after which the data is released under a FOSS license.

Of course, the public wiki should always come first.
_____________________________________________________________________________________________________________________________________
_____________________________________________________________________________________________________________________________________
```