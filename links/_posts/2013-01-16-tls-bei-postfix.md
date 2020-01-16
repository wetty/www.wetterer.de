---

title: "TLS bei Postfix"
date: 2013-01-16 18:04
comments: true
share: true
link: http://forum.parallels.com/showthread.php?t=106832
categories: 
- Links
- Plesk
- Postfix
---
{% include wetty/webshot.html %} Postfix bei Plesk 11 erfordert eine TLS Verbindungsverschlüsselung. Einige einfache eMail Clients, wie sie in Geräten wie Druckern oder Datenloggern vorkommen, scheinen damit ein Problem zu haben. Im [Parallels Forum](http://forum.parallels.com/showthread.php?t=106832) fand sich die Lösung.

Edit /etc/postfix/master.cf file

Original Value is like that:

    submission inet n - - - - smtpd -o smtpd_enforce_tls=yes -o smtpd_tls_security_level=encyrpt-o smtpd_sasl_auth_enable=yes -o smtpd_client_restrictions=permit_sasl_authenticate d,reject -o smtpd_sender_restrictions= -o smtpd_proxy_filter=127.$

Change it as like as this one

    submission inet n - - - - smtpd -o smtpd_enforce_tls=no -o smtpd_tls_security_level=may -o smtpd_sasl_auth_enable=yes -o smtpd_client_restrictions=permit_sasl_authenticate d,reject -o smtpd_sender_restrictions= -o smtpd_proxy_filter=127.$

Then start postfix, that removes STARTTLS requirement at postfix submission service. 
