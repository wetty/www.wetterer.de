---
title: "MP3 Player"
order: 4
description: "Sammlung meiner MP3 Player."
permalink: /sonstiges/mp3/
--- 
{% assign mp3 = site.mp3 | sort: "order" %}

Es fing mit dem aus einem alten PC gebauten [{{ mp3[0].title }}]({{ mp3[0].url }}) (MP3 Audio Player) an. Und setzte sich dann über einen kleinen portablen [{{ mp3[1].title }}]({{ mp3[1].url }}) bis zur [{{ mp3[2].title }}]({{ mp3[2].url }}) fort. 

{% for player in mp3 reversed %}
  * [{{ player.title }}]({{ player.url }}){% endfor %}
  

