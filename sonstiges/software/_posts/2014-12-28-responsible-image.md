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
	    <source srcset="{{ site.url }}/assets/images/grey.gif" data-srcset="//placehold.it/716x476 1x, //placehold.it/1432x952 2x" media="(min-width: 35.563em)" type="image/gif" />
	    <source srcset="{{ site.url }}/assets/images/grey.gif" data-srcset="//placehold.it/516x343 1x, //placehold.it/1032x686 2x" media="(min-width: 20.063em)" type="image/gif" />
	    <img data-srcset="//placehold.it/268x178" class="lazyload" itemprop="image" data-sizes="auto" alt="Responsive Image" src="data:image/gif;base64,R0lGODlhAQABAAAAACH5BAEKAAEALAAAAAABAAEAAAICTAEAOw==" />
	  </picture>
	  <figcaption>Das Bild sollte sich der Auflösung anpassen.</figcaption>
</figure>
<noscript>
    <img src="//placehold.it/716x480" alt="Placehold.it Test" />
</noscript>


<img
	data-sizes="auto"
    data-src="//placehold.it/600x400 600w"
	data-srcset="//placehold.it/600x400 600w,
	    //placehold.it/220x110 220w,
	    //placehold.it/300x150 300w,
	    //placehold.it/600x400 600w,
	    //placehold.it/900x450 900w"
	class="lazyload" />
	
Nachdem ich an einem neuen Layout für meine Homepage arbeite, sollen die Bilder sich auch der Größe des Displays anpassen.

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