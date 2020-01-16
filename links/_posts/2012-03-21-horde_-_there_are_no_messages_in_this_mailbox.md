---

title: "Horde - There are no messages in this mailbox."
date: 2012-03-21 09:44
comments: true
share: true
categories: 
- Links
- Plesk
- Horde
link: http://www.xpcwebhosting.com/2012/horde-webmail-error-there-are-no-messages-in-this-mailbox/
---
{% include wetty/webshot.html %} In Horde Webmail ist ab und an die Inbox leer, obwohl definitiv Mails da sind. Dann wird die Meldung "There are no messages in this mailbox." angezeigt.

Nach etwas Recherche steht fest, dass sich Horde wohl beim speichern der Sortierungsreihenfolge in der Datenbank etwas vertut, und demnach nichts mehr angezeigt wird.

Die Lösung besteht darin die Sortierungspräferenzen des Users in der Datenbank wieder auf den default Wert zu setzen.

    update horde_prefs set pref_value=’a:0:{}’ where pref_uid=’USERNAME‘ and pref_name=’sortpref’ and pref_scope=’imp’;

Die Lösung fand ich auf der folgenden Seite:

[Horde - There are no messages in this mailbox.](http://www.xpcwebhosting.com/2012/horde-webmail-error-there-are-no-messages-in-this-mailbox/)
