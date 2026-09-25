## About

Listiary is a free and open-source wiki engine built around nested lists. Beyond its core purpose, it explores a number of design choices that differ from those of conventional wiki platforms. These choices are intentional: Listiary is a platform for experimenting with different approaches to creating, organizing, and sharing knowledge.

Below are some of its most prominent design principles, divided into core foundations and experimental features.

### Core foundations

**Language for Lists** – Listiary has its own small language for writing lists, called Describe. It is designed to be readable and consistent, without feeling like programming.

**Plain Tech Stack** – Listiary is built with vanilla JavaScript and PHP, with minimal use of self-hosted libraries. This keeps the platform lightweight, reduces external dependencies, and makes its code easier to audit.

**FOSS** – Both Listiary and Describe are free and open source, licensed under AGPL v3.

### Experimental features

**Personal Tool** – Listiary can be used for personal as well as public knowledge. Think of it as an encyclopedia and a notebook, built on top of the same system.

**Extensible** – Listiary supports plugins, including a selection of ready-made ones. Admins can enable or disable them per wiki instance, as well as develop their own.

**Bot-Derived Content** – Wiki admins can run bots that gather information from reputable sources and create articles. Such content can be designated with a low-trust level, reflecting its automated origin and allowing it to be evaluated accordingly.

**Distributed and Sustainable** – Users choose which servers and content to load, giving Listiary a decentralized model. Its architecture is designed with client-side federation, high availability, and asynchronous data synchronization in mind. This flexibility opens up different possibilities for moderation, resilience, and long-term sustainability beyond rigid, centralized platforms.

**Interactive Editing** – Users can customize, edit, highlight, and sort public or personal lists. They can save versioned drafts, fork lists into their own versions, and share them on social media.

**Importable and Exportable** – Listiary does not aim to be the ultimate personal list-making app. Instead, it aims to be a capable list-making tool built on top of a knowledge system. Interoperability matters, so importing and exporting content are priorities wherever possible.

**Forkable Content** – Listiary adopts the GitHub mentality for lists: every list can become the starting point for another. Users can make their own edits, maintain multiple versions, and let them evolve independently.

**Liquid Trust** – Listiary uses a flexible, layered trust model. Users can write freely, while articles receive evolving trust assessments rather than relying on a rigid, binary distinction between trusted and untrusted content.
