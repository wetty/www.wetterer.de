---
title: "Upgrade auf Lexware Buchhalter 18.50"
date: 2013-09-25T14:22:12+02:00
categories: 
- Windows
---
Nachdem ich nun seit Wochen die Update CD für den Lexware Buchhalter auf Version 18.50 mit SEPA Unterstützung hier liegen hab, ging es heute ans installieren.
Nach fast 2 Stunden ist mir das dann auch endlich gelungen. Zuvor gab es einige Hindernisse.

Mein System sieht wie folgt aus: 

  * Mac Book Pro Retina mit 16GB
  * Parallels Desktop 9, frisch upgedatet
  * Windows 7 64Bit Ultimate, alle Updates, kein Virenscanner aktiv
  * Buchhalter 18.04 installiert und funktionsfähig

Nach einlegen der Update CD, Eingabe der Seriennummer kommt irgendwann bei 3% der Installation die Meldung: 

    Die Rechte vom Installer reichen nicht aus, um auf diesen Ordner zuzugreifen: C:\Program Files (x86)\Common Files\RemoteSupport. Die Installation kann nicht fortgesetzt werden. Melden Sie sich als Administrator an oder wenden Sie sich an Ihren Systemadministrator.

{% include wetty/image.html class="center" path="/assets/images/fehlerlexwaresetup.png" %}

Da ich selbst der Administrator bin, musste ich mich wohl oder übel auch selbst darum kümmern.

Die Installation wurde abgebrochen, mit dem Erfolg, das auch meine bislang funktionierende Buchhalter Installation deinstalliert war. Glücklicherweise hatte Parallels vorher einen Snapshot meiner Windows Installation erstellt, womit ich den Ausgangszustand leicht wieder herstellen konnte.

Der Versuch den genannten Ordner mit entsprechenden Rechten auszustatten scheiterte ebenfalls, da ich dazu keine Rechte hatte.

Also zurück zum letzten Snapshot und die kostenlose Hotline angerufen. Erste Information war, das Installationen auf einem Windows in einer virtuellen Maschine normal nicht supported würden. Aber ich solle mal einen Ordner auf dem Windows Desktop erstellen und den gesamten Inhalt der CD dort hinein kopieren. Danach die Installation aus diesem Ordner heraus durchführen. Kurzum, das klappte auch nicht.

Schlussendlich kam ich zum Ziel, indem ich dem genannten Ordner vor der Installation Vollzugriff für folgende Gruppen gab:

- ERSTELLER-BESITZER
- SYSTEM
- Administratoren
- Benutzer
- TrustedInstaller

Danach lief die Installation dann ohne Probleme durch.

