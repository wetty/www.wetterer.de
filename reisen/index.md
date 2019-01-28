---
title: Reisen
description: "Archiv aller Reiseberichte."
---

<ul class="post-list">{% for post in site.tags.ReiseStart %}
<li><article><a href="{{ site.url }}{{ site.baseurl }}/{{ post.categories[0] }}/{{ post.categories[1] }}/">{{ post.title }} <span class="entry-date"><time datetime="{{ post.date | date_to_xmlschema }}">{% include wetty/mydate.html %}</time></span>{% if post.excerpt %} <span class="excerpt">{{ post.excerpt | strip_html | strip_newlines | truncate: 60,'...' | replace:'[','' | replace:']','' }}</span>{% endif %}</a></article></li>{% endfor %}</ul>