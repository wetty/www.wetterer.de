---
title: "Sonstiges"
subtitle: "Oder alles was keinen Platz im Menu gefunden hat"
permalink: /sonstiges/
description: "Alles was kein Platz im Menu gefunden hat."
--- 
{% assign sonstiges = site.sonstiges | sort: "order" %}


{% for son in sonstiges %}
  * [{{ son.title }}]({{ son.url }}): {{ son.description }}{% endfor %}
	
## Blogroll
  * [Geek & Poke](https://geek-and-poke.com/){: target="_blank" rel="noopener noreferrer nofollow"}: Beste Comic Serie überhaupt. Nur für Entwickler zu verstehen.
  * [Moby Dick III](https://www.moby-dick.de){: target="_blank" rel="noopener noreferrer nofollow"}: Rund um die Segelyacht, mit der ich öfter unterwegs bin.

