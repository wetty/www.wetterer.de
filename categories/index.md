---
title: Kategorien
description: "Hier finden sich alle Kategorien, die hier auf der Website vorkommen."
---

{% capture site_tags %}{% for tag in site.categories %}{{ tag | first }}{% unless forloop.last %},{% endunless %}{% endfor %}{% endcapture %}
{% assign tags_list = site_tags | split:',' | sort %}

<ul class="tag-box inline">
  {% for item in (0..site.categories.size) %}{% unless forloop.last %}
    {% capture this_word %}{{ tags_list[item] | strip_newlines }}{% endcapture %}
    <li><a href="#{{ this_word }}">{{ this_word }} <span>{{ site.categories[this_word].size }}</span></a></li>
  {% endunless %}{% endfor %}
</ul>

{% for item in (0..site.categories.size) %}{% unless forloop.last %}
  {% capture this_word %}{{ tags_list[item] | strip_newlines }}{% endcapture %}
  <h2 id="{{ this_word }}">{{ this_word }}</h2>
  <ul class="post-list">{% for post in site.categories[this_word] %}{% if post.title != null %}{% include wetty/post-list.html %}{% endif %}{% endfor %}</ul>
{% endunless %}{% endfor %}