---
title: "Suche"
search_omit: true
sitemap: false
permalink: /search/
description: Hier läßt sich nach allen Artikel Überschriften suchen. 
---
  
<!-- Search form -->
<form method="get" action="{{ site.url }}/search/" data-search-form class="simple-search">
  <label for="q">Durchsuche {{ site.title }}:</label>
  <input type="search" name="q" id="q" placeholder="Nach was suchen Sie?" data-search-input id="goog-wm-qt" />
  <input type="submit" value="Suchen" id="goog-wm-sb" />
</form>

<!-- Search results placeholder -->
<h6 data-search-found>
  <span data-search-found-count></span> Ergebnisse gefunden für &ldquo;<span data-search-found-term></span>&rdquo;.
</h6>
<ul class="post-list" data-search-results></ul>

<!-- Search result template -->
<script type="text/x-template" id="search-result">
  <li><article>
    <a href="##Url##">##Title## <span class="excerpt">##Excerpt##</span></a>
  </article></li>
</script>
