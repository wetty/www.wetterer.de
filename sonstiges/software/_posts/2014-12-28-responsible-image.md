---
title: "Responsible Image"
date: 2014-12-28T17:47:25+01:00
tags: [Responsive Design]
---
<figure class="photo-with-exif">
	<picture>
<!-- Home Settings
	    <source srcset="http://placehold.it/908x448" media="(min-width: 48.063em)" type="image/gif" />
	    <source srcset="http://placehold.it/716x480" media="(min-width: 40.063em)" type="image/gif" />
-->
<!-- Blog Page Settings
		<source srcset="http://placehold.it/715x448" media="(min-width: 62.5em)" type="image/gif" />
	    <source srcset="http://placehold.it/908x480" media="(min-width: 48.063em)" type="image/gif" />
	    <source srcset="http://placehold.it/716x480" media="(min-width: 37.5em)" type="image/gif" />
-->
<!--
		<source src="{{ site.url }}/assets/images/grey.gif" data-srcset="http://placehold.it/715x448" media="(min-width: 62.5em)" type="image/gif" />
	    <source src="{{ site.url }}/assets/images/grey.gif" data-srcset="http://placehold.it/908x480" media="(min-width: 48.063em)" type="image/gif" />
-->
	    <source srcset="{{ site.url }}/assets/images/grey.gif" data-srcset="//placehold.it/936x468 1x, //placehold.it/1872x936 2x" media="(min-width: 1281px)" />
	    <source srcset="{{ site.url }}/assets/images/grey.gif" data-srcset="//placehold.it/1024x512 1x, //placehold.it/2048x1024 2x" media="(min-width: 1025px)" />
	    <source srcset="{{ site.url }}/assets/images/grey.gif" data-srcset="//placehold.it/972x486 1x, //placehold.it/1944x972 2x" media="(min-width: 901px)" />
	    <source srcset="{{ site.url }}/assets/images/grey.gif" data-srcset="//placehold.it/848x424 1x, //placehold.it/1696x848 2x" media="(min-width: 769px)" />
	    <source srcset="{{ site.url }}/assets/images/grey.gif" data-srcset="//placehold.it/732x366 1x, //placehold.it/1464x732 2x" media="(min-width: 601px)" />
	    <source srcset="{{ site.url }}/assets/images/grey.gif" data-srcset="//placehold.it/553x275 1x, //placehold.it/1106x550 2x" media="(min-width: 415px)" />
	    <source srcset="{{ site.url }}/assets/images/grey.gif" data-srcset="//placehold.it/379x175 1x, //placehold.it/718x350 2x" media="(min-width: 376px)" />
	    <source srcset="{{ site.url }}/assets/images/grey.gif" data-srcset="//placehold.it/343x172 1x, //placehold.it/686x344 2x" media="(min-width: 361px)" />
	    <source srcset="{{ site.url }}/assets/images/grey.gif" data-srcset="//placehold.it/328x164 1x, //placehold.it/656x328 2x" media="(min-width: 321px)" />
	    <img data-srcset="//placehold.it/288x178 1x, //placehold.it/576x356 2x " class="lazyload" itemprop="image" data-sizes="auto" alt="Responsive Image" src="data:image/gif;base64,R0lGODlhAQABAAAAACH5BAEKAAEALAAAAAABAAEAAAICTAEAOw==" />
	  </picture>
	  <figcaption>Das Bild sollte sich der Auflösung anpassen.</figcaption>
</figure>
<noscript>
    <img src="//placehold.it/716x480" alt="Placehold.it Test" />
</noscript>

<figure class="">
<a href="//placehold.it/1024x512" class="{{ site.image_popup_class }}" title="{{ include.alt }}">
<img
	data-sizes="auto"
    data-src="//placehold.it/288x178 288w"
	data-srcset="//placehold.it/936x468 936w,
//placehold.it/1024x512 1024w,
//placehold.it/972x486 972w,
//placehold.it/848x424 848w,
//placehold.it/732x366 732w,
//placehold.it/553x275 553w,
//placehold.it/379x175 379w,
//placehold.it/343x172 343w,
//placehold.it/328x164 328w"
	class="lazyload" />
</a>
<figcaption>Responsive Test</figcaption>
</figure>
	
Nachdem ich an einem neuen Layout für meine Homepage arbeite, sollen die Bilder sich auch der Größe des Displays anpassen.

<figure class="align-right">
<a href="//placehold.it/1024x512" class="{{ site.image_popup_class }}" title="test">
<img
	data-sizes="auto"
    data-src="//placehold.it/288x178 288w"
	data-srcset="//placehold.it/936x468 936w,
//placehold.it/1024x512 1024w,
//placehold.it/972x486 972w,
//placehold.it/848x424 848w,
//placehold.it/732x366 732w,
//placehold.it/553x275 553w,
//placehold.it/379x175 379w,
//placehold.it/343x172 343w,
//placehold.it/328x164 328w"
	class="lazyload" />
</a>
</figure>

<figure class="half">
<a href="//placehold.it/1024x512" class="{{ site.image_popup_class }}" title="test">
<img src="data:image/gif;base64,R0lGODlhAQABAAAAACH5BAEKAAEALAAAAAABAAEAAAICTAEAOw==" data-src="{{ site.url_cloudinary_width }}{{ member.image }}" class="lazyload" alt="{{ member.alt }}" data-sizes="auto" data-widths="[25, 50, 75, 100, 150, 200, 250, 300, 350, 400, 450]" />
<img
	data-sizes="auto"
    data-src="//placehold.it/288x178 288w"
	data-srcset="//placehold.it/150x75 150w,
//placehold.it/100x50 100w,
//placehold.it/75x35 75w,
//placehold.it/50x25 50w,
//placehold.it/25x12 25w"
	class="lazyload" />
</a>
<a href="//placehold.it/1024x512" class="{{ site.image_popup_class }}" title="test">
<img src="data:image/gif;base64,R0lGODlhAQABAAAAACH5BAEKAAEALAAAAAABAAEAAAICTAEAOw==" data-src="{{ site.url_cloudinary_width }}{{ member.image }}" class="lazyload" alt="{{ member.alt }}" data-sizes="auto" data-widths="[25, 50, 75, 100, 150, 200, 250, 300, 350, 400, 450]" />
<img
	data-sizes="auto"
    data-src="//placehold.it/288x178 288w"
	data-srcset="//placehold.it/150x75 150w,
//placehold.it/100x50 100w,
//placehold.it/75x35 75w,
//placehold.it/50x25 50w,
//placehold.it/25x12 25w"
	class="lazyload" />
</a>
</figure>

<!--
Max width 360 Bild 328
320 - 288
360 - 328
375 - 343
411 - 379
414 - 382
600 - 553
768 - 732
1024 - 784
-->

<!--
// MEDIA QUERIES ==============================================
$micro            : "only screen and (min-width: 30em)";
$small            : "only screen and (min-width: 37.5em)";
$medium           : "only screen and (min-width: 48em)";
$large            : "only screen and (min-width: 62em)";
$x-large          : "only screen and (min-width: 86.375em)";

48em 768px
48.063em 769px
20em 320px
35.5em 568px

// Small screens 
@media only screen { } /* Define mobile styles */ 
@media only screen and (max-width: 40em) { } /* max-width 640px, mobile-only styles, use when QAing mobile issues */ 
// Medium screens 
@media only screen and (min-width: 40.063em) { } /* min-width 641px, medium screens */ @media only screen and (min-width: 40.063em) and (max-width: 64em) { } /* min-width 641px and max-width 1024px, use when QAing tablet-only issues */ // Large screens @media only screen and (min-width: 64.063em) { } /* min-width 1025px, large screens */ @media only screen and (min-width: 64.063em) and (max-width: 90em) { } /* min-width 1025px and max-width 1440px, use when QAing large screen-only issues */ 
// XLarge screens @media only screen and (min-width: 90.063em) { } /* min-width 1441px, xlarge screens */ @media only screen and (min-width: 90.063em) and (max-width: 120em) { } /* min-width 1441px and max-width 1920px, use when QAing xlarge screen-only issues */ // XXLarge screens @media only screen and (min-width: 120.063em) { } /* min-width 1921px, xxlarge screens */
-->