---
title: "Upgrade auf Lexware Buchhalter 2014"
date: 2013-11-20T13:49:46+02:00
tags:
- Windows
---
Kaum 8 Wochen nach meinen Update Problem auf die Lexware Buchhalter Version 18.50, steh ich nun wieder vor dem gleichen Problem beim Update auf Lexware Buchhalter 2014.

{% include wetty/image.html class="center" path="/assets/images/fehlerlexwaresetup2014.png" width=620 height=581 %}

Diesmal war ich vorbereitet. Nach dem Problem den Snapshot meiner virtuellen Maschine zurück gespielt, die Rechte des genannten Ordners geändert und vor der Installation Vollzugriff für folgende Gruppen gegeben:

- ERSTELLER-BESITZER
- SYSTEM
- Administratoren
- Benutzer
- TrustedInstaller

Und schon lief die Installation ohne Probleme durch.

