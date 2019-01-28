---
title: "Links"
order: 3
description: "Sammlung aller externen Links."
---
## Links
<ul class="post-list">
{% for post in site.categories.links %}
<li><article><a href="{{ site.url }}{{ site.baseurl }}{{ post.url }}">{{ post.title }} <span class="entry-date"><time datetime="{{ post.date | date_to_xmlschema }}">{% include wetty/mydate.html %}</time></span></a>
<span class="excerpt">
	<a href="{{ post.link }}">{{ post.link }}</a> {% include wetty/webshot.html param=post.link %}
</span>
</article></li>
{% endfor %}</ul>
