---
title: "Welcome to my blog"
date: 2022-10-17T22:48:08+02:00
draft: true
toc: true
image: cover.jpg
description: 
categories: dev   

---


Dies ist nun mein nächster Versuch nach fast einem Jahrzehnt wieder eine persönlche Webseite mit eigenem Blog online zu stellen. Es soll als Dokumentation meiner eigenen Erkentnisse für mich und andere dienen. Die üblichen beliebten Dienste wie Medium oder Squarespace usw. kamen nicht in Frage, weil ich durch Selbsthosting die Individualität und Unabhängigkeit des Internets noch Wertschätzung zeigen möchte.
Aufgrund von Zeitmangel muss der Aufwand trotz Eigenhosting so gering wie möglich gehalten werden, deswegen wurde es nicht wie so üblichen ein CMS wie Wordpress. Ich habe mich für Hugo entschieden, das ein [JamStack-Ansatz](https://jamstack.org/) verfolgt und gute Themes bereitstellt und von der Struktur her sich an Software-Dokumentation anlehnt.

Wenn man bei der Software-Entwicklung Texte für die Dokumentation in seiner liebgewonnen IDE und in Markdown verfasst, so muss man beim bloggen aus dieser Routine nicht ausbrechen und sich nicht in irgendwelchen CMS einloggen und sich mit WYSIWYG-Editoren rumschlagen.

## MkDocs vs Hugo

Zuerst hatte ich mich für [MkDocs](https://www.mkdocs.org/) entschieden. Es ist ein in Python implementierter Static Site Generator den man mit Markdown-Dokumenten füttert und der daraus eine HTML-Seite generiert. Konfriguiert wird es in YAML und für die HTML-Templates wird die [Jinja engine](https://jinja.palletsprojects.com/en/3.1.x/) verwendet. Durch fertige Themes bekommt man so schnell ansprechende Webseiten als Ergebniss, darunter das wohl beliebteste [Material for MkDocs ](https://squidfunk.github.io/mkdocs-material/). Wie der Name schon andeutet, baut es auf das [Material-Design](https://m2.material.io/design/) auf und bietet ganz nützliche Plugins, wie die Suche und Social-Media-Cards. Es hat auch ein eingebautes [Blog-Plugin](https://squidfunk.github.io/mkdocs-material/setup/setting-up-a-blog/#built-in-blog-plugin), das aber nur für "Insiders" nutzbar ist. Insiders ist [jeder der den Entwickler mit mindestens 15 Euro im Monat unterstützt](https://squidfunk.github.io/mkdocs-material/insiders/#what-is-insiders). Der Entwickler hat sicherlich viel Arbeit reingesteckt, für eine kleine private Webseite ist das aber ein unverhältnismäßiger hoher Betrag.

Unzufrieden mit diesem Umstand, habe ich weiter gesucht und dann [Hugo](https://gohugo.io/) entdeckt. Auf dieser Seite findet man eine Liste von vielen [Static Site Generetoren](https://jamstack.org/generators/) und kann sich selbst einen Eindruck von der Großen Auswahl machen.


This webpages are static generated markdown documents that are generated from my github repository.
A push or merge to the master branch triggers a github action that starts the [Hugo](https://gohugo.io/) static site generator, witch builds this whole website and puts the static html documents inside an own branch. I use the github webpage hosting service and my own domain to serve the html documents to the internet.

The benifits of this approach are:

* free webhosting through github pages
* Using git and markdown workflow to write/edit and deploy your content
* No maintenance for a CMS like wordpress, no security updates, no bugs, no hacks
* Third part contribution with pull requests

![Die Darstellung meines Editors](editor.png)

