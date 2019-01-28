---
title: Blog Archiv
description: "Archiv aller Blog Posts"
permalink: /archives/
search_omit: true
---
<ul class="post-list">{% for post in site.posts %}{% include wetty/post-list.html %}{% endfor %}</ul>