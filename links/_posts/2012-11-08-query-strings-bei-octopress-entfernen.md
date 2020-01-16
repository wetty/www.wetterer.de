---

title: "Query strings bei Octopress entfernen"
date: 2012-11-08 08:23
comments: true
share: true
link: http://www.pacbard.tk/2012/10/27/remove-query-strings-from-octopress-assets/ 
categories: 
- Links
- Octopress
---
{% include wetty/webshot.html %} Bei Bildern wurde immer ein query string angehängt, was teilweise das cachen dieser Bilder verhindert. Hier nun ein Tipp, wie man das abstellen kann. 

[Query strings bei Octopress entfernen](http://www.pacbard.tk/2012/10/27/remove-query-strings-from-octopress-assets/)

``` ruby config.rb
# Disable query string in compass
asset_cache_buster :none
```