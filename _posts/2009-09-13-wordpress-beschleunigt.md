---
title: "Wordpress beschleunigt"
date: 2009-09-13 20:46
---
Heute Abend war mal etwas Zeit sich um die Technik meines Wordpress Blogs zu kümmern. Der Aufbau der Seiten war nicht wirklich schnell.

Das Tool meiner Wahl war YSlow, ein Firefox Plugin, mit welchem sich unter anderem die Zeit messen läßt, die eine Website zum laden braucht. Weiterhin läßt sich damit detailiert feststellen, was genau an der Seite wie lange braucht. Die erste Messung ergab eine Zeit von über vier Sekunden. Das mußte geändert werden. Die ersten Einstellungen führte im am Server durch, um die ETags abzuschalten, und eine expiry header hinzuzufügen.

<!--more-->

Als nächstes hatte ich mir die Javascripte vorgenommen. Hier im besonderen die Platzierung der Scripte. Viele Scripte werden bereits am Anfang der Seite geladen. Performanter ist es allerdings die Skripte erst am Ende der Seite zu laden. Darauf macht einem ebenfalls YSlow aufmerksam. Wordpress bietet den Plugins bereits die Option an, die Skripte im Footer laden zu lassen. Leider nutzen das noch wenige meiner eingesetzten Plugins. Nach einigen Änderungen in diversen PHP Dateien erschien tatsächlich das ein oder andere im Footer.

Da Wordpress etliche Datenbankzugriffe für eine einzelne Seite macht, galt es diesen Vorgang zu verbessern. Hier griff ich der einfachheit auf WP-Super-Cache zurück. Die Seiten werden damit einmal erstellt, und für eine gewisse Zeit in einem Cache abgelegt. Von dort können sie dann sehr schnell wieder abgerufen werden. Diese Maßnahme reduzierte den Aufbau der Seiten auf rund 1,8 Sekunden. Zwar schon mehr als über die hälfte weniger, aber es könnte ruhig noch schneller gehen.

YSlow zeigte dann eine CSS Datei, die alleine bereits 0,8 Sekunden beanspruchte. Wie sich heraus stellte war das eine PHP Datei, die wohl das CSS für den Wordpress Flickr Manager generiert. Da sich dort wohl nicht viel ändert, ist mir etwas unklar, warum das Stylesheet dynamisch generiert wird. Kurzerhand hab ich das PHP entfernt, und durch ein statisches CSS ersetzt.

Nach allen diesen Anpassungen brauchen meine Wordpress Seiten nun mit Cache unter eine Sekunde. Alles in allem konnte ich somit über 3 Sekunden, sprich dreiviertel der anfänglichen Gesamtzeit wegoptimieren.
