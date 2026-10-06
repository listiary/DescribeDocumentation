---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults

layout: page
title:
# permalink: /listiary/
exclude: true
---
<style>
  .hero-logo {
    max-width: 70%;
    height: auto;
    display: block;
    margin: auto;
  }

  @media (max-width: 768px) {
    .hero-logo {
      max-width: 100%;
    }
  }
</style>
<br>
<img src="{{ site.baseurl }}/assets/images/listiary.png" alt="logo" class="hero-logo">
<br><br><br>
Listiary is an experimental wiki project built around lists rather than articles. The basic idea is simple: lists are treated as their own kind of object, not as formatting inside text. That decision shapes most of the system, from how content is written to how it changes over time.
<br><br>

### About
Listiary is a free and open-source wiki engine built around nested lists. Beyond its core purpose, it explores a number of design choices that differ from those of conventional wiki platforms. These choices are intentional: Listiary is a platform for experimenting with different approaches to creating, organizing, and sharing knowledge.<br>

Below are some of its most prominent design principles, divided into core foundations and experimental features.<br>
<br><br>

### Core foundations
Language for Lists – Listiary has its own small language for writing lists, called Describe. It is designed to be readable and consistent, without feeling like programming.<br>

Plain Tech Stack – Listiary is built with vanilla JavaScript and PHP, with minimal use of self-hosted libraries. This keeps the platform lightweight, reduces external dependencies, and makes its code easier to audit.<br>

FOSS – Both Listiary and Describe are free and open source, licensed under AGPL v3.<br>
<br><br>

### Experimental features
Personal Tool – Listiary can be used for personal as well as public knowledge. Think of it as an encyclopedia and a notebook, built on top of the same system.<br>

Extensible – Listiary supports plugins, including a selection of ready-made ones. Admins can enable or disable them per wiki instance, as well as develop their own.<br>

Bot-Derived Content – Wiki admins can run bots that gather information from reputable sources and create articles. Such content can be designated with a low-trust level, reflecting its automated origin and allowing it to be evaluated accordingly.<br>

Distributed and Sustainable – Users choose which servers and content to load, giving Listiary a decentralized model. Its architecture is designed with client-side federation, high availability, and asynchronous data synchronization in mind. This flexibility opens up different possibilities for moderation, resilience, and long-term sustainability beyond rigid, centralized platforms.<br>

Interactive Editing – Users can customize, edit, highlight, and sort public or personal lists. They can save versioned drafts, fork lists into their own versions, and share them on social media.<br>

Importable and Exportable – Listiary does not aim to be the ultimate personal list-making app. Instead, it aims to be a capable list-making tool built on top of a knowledge system. Interoperability matters, so importing and exporting content are priorities wherever possible.<br>

Forkable Content – Listiary adopts the GitHub mentality for lists: every list can become the starting point for another. Users can make their own edits, maintain multiple versions, and let them evolve independently.<br>

Liquid Trust – Listiary uses a flexible, layered trust model. Users can write freely, while articles receive evolving trust assessments rather than relying on a rigid, binary distinction between trusted and untrusted content.<br>

<br><br>
### Links
[Project Listiary](/listiary/)<br>
[Project Describe](/language/)<br>
<br>
[subpr. Describe Library](https://library.listiary.org/)<br>
[subpr. Documentation](/listiary/documentation/home/)<br>
[subpr. Documedia](https://documedia.listiary.org/)<br>
[subpr. Maps](/listiary/maps/)<br>
[subpr. Articles](/listiary/articles/)<br>
