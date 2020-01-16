---
title: "Sonstiges"
permalink: /sonstiges/
description: "Alles was kein Platz im Menu gefunden hat."
--- 
{% assign sonstiges = site.sonstiges | sort: "order" %}

## Sonstiges 

{% for son in sonstiges %}
  * [{{ son.title }}]({{ son.url }}): {{ son.description }}{% endfor %}
	
## Blogroll
  * [Geek & Poke](http://geek-and-poke.com/): Beste Comic Serie überhaupt. Nur für Entwickler zu verstehen.
  * [Moby Dick III](http://www.moby-dick.de): Rund um die Segelyacht, mit der ich öfter unterwegs bin.

