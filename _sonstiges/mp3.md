---
title: "MP3 Player"
order: 4
description: "Sammlung meiner MP3 Player."
--- 
{% assign mp3 = site.mp3 | sort: "order" %}

Es fing mit dem aus einem alten PC gebauten [{{ mp3[0].title }}]({{ site.url }}{{ mp3[0].url }}) (MP3 Audio Player) an. Und setzte sich dann über einen kleinen portablen [{{ mp3[1].title }}]({{ site.url }}{{ mp3[1].url }}) bis zur [{{ mp3[2].title }}]({{ site.url }}{{ mp3[2].url }}) fort. 

{% for player in mp3 reversed %}
  * [{{ player.title }}]({{ site.url }}{{ player.url }}){% endfor %}
  

