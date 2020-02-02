---
title: "Diese Datei befindet sich außerhalb Ihres lokalen Netzwerkes..."
date: 2013-08-21T10:13:33+02:00
link: http://www.naggy.de/archives/97-Access-Fehler-Diese-Datei-befindet-sich-ausserhalb-Ihres-Intranets-oder-auf-einer-Webseite.html
tags: [Windows]
---
Vor Jahren hatte ich schonmal versucht, die lästige Windows Meldung, die man beim starten von ausführbaren Dateien von einem Netzwerklaufwerk erhält, zu vermeiden.

> "Diese Datei befindet sich außerhalb Ihres lokalen Netzwerkes. Dateien von unbekannten Speicherorten können Ihren PC beschädigen."

Damals hies es dann, das sei nicht möglich, und die Meldung würde immer kommen.

Jedenfalls kam das Thema gestern wieder auf, nachdem die Finanz Software [SFirm](http://www.sfirm.de/) wohl aus einigen einzelnen ausführbaren Modulen besteht, und somit bei jeder Aktion diese Meldung hoch kommt.

Die Lösung liegt nun darin im Internet Explorer unter den **Interneteinstellungen** bei **Sicherheit** im **Lokales Intranet** die Automatik abzuschalten und **Alle Netzwerkpfade (UNCs) einbeziehen** auszuwählen. Dann unter **Erweitert...** einfach den Pfad, bzw. geht auch die IP Adresse des Laufwerks, einzutragen und der lokalen Intranet Zone hinzuzufügen.

Und siehe da, selbst ohne Neustart des Rechners, ist diese Meldung endlich verschwunden.
 