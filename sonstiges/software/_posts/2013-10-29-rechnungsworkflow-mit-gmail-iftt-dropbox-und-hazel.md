---
title: Rechnungsworkflow mit gmail, ifttt, Dropbox und Hazel
date: 2013-10-29 10:58
tags:
- OSX
- Workflow
---
Die meisten regelmässigen Rechnungen kommen mittlerweile ja als PDF Anhang per Email. Normalerweise geht man her und speichert sich diese PDF Rechnung irgendwo auf seinem Rechner ab und/oder druckt sich diese aus. Da die Rechnungen meist kryptische Namen haben, ändert man den beim speichern der PDF Datei noch entsprechend ab, dass man die Rechnung besser findet.

Das alles lässt sich wunderbar automatisieren, so dass man sich nicht mehr um das korrekte ablegen der Rechnungen kümmern muss. Mein Workflow für das ganze sieht derzeit wie folgt aus.

Mit [IFTTT]{: target="_blank" rel="noopener noreferrer"} gibt es einen wunderbaren Service im Internet, der verschiedene Internet Kanäle im Hintergrund beobachtet und bei bestimmten Ereignisse dann entsprechende Aufgaben ausführt. Nachdem meine emails alle über [Google Mail]{: target="_blank" rel="noopener noreferrer"} laufen, lass ich IFTTT alle neuen emails auf Anhänge checken und dann die Anhänge in meine [Dropbox]{: target="_blank" rel="noopener noreferrer"} speichern. Jeweils in Unterordner, die den Absender wieder spiegeln.

[Hazel]{: target="_blank" rel="noopener noreferrer"} macht dann die Automatisierung auf meinem MacBook. Hierzu hab ich ein paar Regeln für Hazel definiert, welche jeweils in die einzelnen Ordner der Absender von Rechnungen in meiner Dropbox nachschauen. Findet sich dort ein PDF, so schaut Hazel in dieses PDF hinein und holt sich das entsprechende Rechnungsdatum dieser Rechnung heraus. Danach nennt Hazel die PDF Datei entsprechende um, z.B. in **Rechnung - 2013-10-28 - sipgate.pdf**. Abschliessend verschiebt Hazel diese Datei dann noch in meinen Rechnungsordner.

Einmal das ganze eingerichtet, was nicht sehr viel Arbeit ist, und man muss sich nie mehr um die Ablage von PDF Rechnungen kümmern, die per email ankommen.

{% include _references.md %}
