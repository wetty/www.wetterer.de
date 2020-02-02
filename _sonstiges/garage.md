---
title: "Garage"
order: 1
description: "Im Laufe der Jahre kamen einige Motorräder zusammen. Einige davon sind längst verkauft, andere davon sind immer noch vorhanden."
permalink: /sonstiges/garage/
redirect_from:
  - /garage/
--- 

{% include wetty/image.html class="center" path="/assets/images/garage/garage.jpg" width=518 height=236 %}

{% assign aktuell = site.garage | where: "type", "aktuell" | sort: "order" %}
{% assign verkauft = site.garage | where: "type", "verkauft" | sort: "order" %}

## Aktuell 
Hier stehen alle Motorräder, die noch in meinem Besitz sind. 

{% for moto in aktuell reversed %}
  * [{{ moto.title }}]({{ moto.url }}){% endfor %}

## Verkauft
Hier stehen alle Motorräder, mit denen ich mal unterwegs war, bzw. die ich mal besessen hab. 

{% for moto in verkauft reversed %}
  * [{{ moto.title }}]({{ moto.url }}){% endfor %}


## Autos mit Geschichte
Über ein Auto gab es auch des öfteren was zu berichten.

  * [Fiat Doblo Cargo Natural Power](/sonstiges/garage/fiat-doblo-cargo-natural-power/)