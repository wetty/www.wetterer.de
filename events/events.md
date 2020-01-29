---
layout: archive
---

{{ content }}

<div class="entries-{{ page.entries_layout }}">
  {% include posts-category.html taxonomy=page.categories[1] type=page.entries_layout %}
</div>
