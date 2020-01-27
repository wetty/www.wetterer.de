---
title: "Greylisting pattern aktiv obwohl entfernt"
date: 2012-03-26 18:34
tags: [Plesk]
link: http://serversupportforum.de/forum/plesk/44604-greylisting-blacklist-pattern-noch-aktiv-obwohl-entfernt.html
---
{% include wetty/webshot.html %} Noch ein Problem bei Plesk und Greylisting, was sich mit dem Tipp endlich lösen lies.

[Greylisting pattern aktiv obwohl entfernt](http://serversupportforum.de/forum/plesk/44604-greylisting-blacklist-pattern-noch-aktiv-obwohl-entfernt.html)

Kurzum, die Werte in

    /usr/local/psa/bin/grey_listing --info-server

müßen mit denen in der SQLite DB übereinstimmen

    sqlite3 /var/lib/plesk/mail/greylist/settings.db "select * from remote_domains"
