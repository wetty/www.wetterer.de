---
title: "Responsible Image Test"
date: 2020-01-19T10:38:25+01:00
categories: [Responsive Design]
---

Hier ist ein Bild:

<style>
	.blur-up {
		-webkit-filter: blur(5px);
		filter: blur(5px);
		transition: filter 1400ms, -webkit-filter 1400ms;
	}

	.blur-up.lazyloaded {
		-webkit-filter: blur(0);
		filter: blur(0);
	}

img[data-sizes="auto"] { display: block; width: 100%; }

</style>

<img 
    data-src="https://res.cloudinary.com/demo/image/upload/w_auto,c_scale/smiling_man.jpg" 
	data-sizes="auto"
	width="100vw"
    class="lazyload blur-up cld-responsive" />


Hier eigentlich RIAS
<img
    src="data:image/gif;base64,R0lGODlhAQABAAAAACH5BAEKAAEALAAAAAABAAEAAAICTAEAOw=="
	data-widths="[636, 754, 770, 824, 936, 972, 1022]"
	data-src="//placehold.it/{width}"
	data-sizes="auto"
	class="lazyload"
	alt="" />	

<img
	src="//placehold.it/100"
	data-src="//res.cloudinary.com/dsuwkv08y/image/fetch/q_auto,f_auto,w_{width},c_scale,fl_progressive/https://www.wetterer.de/assets/images/responsive/popup/grillen/Texas-Ranger-Smoker-D71_0251.jpg" 
	data-sizes="auto"
	class="lazyload"
	alt="" />	


Und noch eins
<img
	data-sizes="auto"
	width="100vw"
    data-src="//placehold.it/220"
	data-srcset="//placehold.it/636 636w,
	    //placehold.it/220 220w,
	    //placehold.it/300 300w,
	    //placehold.it/600 600w,
	    //placehold.it/900 900w"
	class="lazyload cld-responsive" />
	
	
hier ein figure Element:

<figure class="photo-with-exif">
	<picture>
        <img
    src="data:image/gif;base64,R0lGODlhAQABAAAAACH5BAEKAAEALAAAAAABAAEAAAICTAEAOw=="
	data-widths="[636, 754, 770, 824, 936, 972, 1022]"
	data-src="//placehold.it/{width}"
	data-sizes="auto"
	class="lazyload"
	alt="" />	
	  </picture>
	  <figcaption>Das Bild sollte sich der Auflösung anpassen.</figcaption>
</figure>

<figure class="photo-with-exif">
	<picture>
	    <source srcset="{{ site.url }}/assets/images/grey.gif" data-srcset="https://placehold.it/636" media="(min-width: 80em)" type="image/gif" />
	    <source srcset="{{ site.url }}/assets/images/grey.gif" data-srcset="https://placehold.it/824" media="(min-width: 64em)" type="image/gif" />
	    <source srcset="{{ site.url }}/assets/images/grey.gif" data-srcset="https://placehold.it/972" media="(min-width: 48em)" type="image/gif" />
	    <img data-srcset="https://placehold.it/720" class="blog-full lazyload cld-responsive" itemprop="image" data-sizes="auto" alt="Responsive Image" src="data:image/gif;base64,R0lGODlhAQABAAAAACH5BAEKAAEALAAAAAABAAEAAAICTAEAOw==" />
	  </picture>
	  <figcaption>Das Bild sollte sich der Auflösung anpassen.</figcaption>
</figure>

<noscript>
    <img src="https://placehold.it/716x480" alt="Placehold.it Test" />
</noscript>

Nachdem ich an einem neuen Layout für meine Homepage arbeite, sollen die Bilder sich auch der Größe des Displays anpassen.

<img 
    data-src="//res.cloudinary.com/dsuwkv08y/image/fetch/q_auto,f_auto,w_auto,c_scale,fl_progressive/https://www.wetterer.de/assets/images/responsive/popup/grillen/Texas-Ranger-Smoker-D71_0251.jpg" 
	data-widths="[636, 754, 770, 824, 936, 972, 1022]"
	data-sizes="auto"
    class="lazyload blur-up cld-responsive">

<img 
    data-src="//res.cloudinary.com/dsuwkv08y/image/fetch/q_auto,f_auto,w_auto,c_scale,fl_progressive/https://www.wetterer.de/assets/images/responsive/popup/grillen/Texas-Ranger-Smoker-D71_0252.jpg" 
	data-sizes="auto"
    class="lazyload blur-up cld-responsive">

<img 
    data-src="//res.cloudinary.com/dsuwkv08y/image/fetch/q_auto,f_auto,w_auto,c_scale,fl_progressive/https://www.wetterer.de/assets/images/responsive/popup/grillen/Texas-Ranger-Smoker-D71_0253.jpg" 
	data-sizes="auto"
	width="100vw"
    class="lazyload blur-up cld-responsive">
<img 
    data-src="//res.cloudinary.com/dsuwkv08y/image/fetch/q_auto,f_auto,w_auto,c_scale,fl_progressive/https://www.wetterer.de/assets/images/responsive/popup/grillen/Texas-Ranger-Smoker-D71_0254.jpg" 
	data-sizes="auto"
	width="100vw"
    class="lazyload blur-up cld-responsive">

<img 
    data-src="//res.cloudinary.com/dsuwkv08y/image/fetch/q_auto,f_auto,w_auto,c_scale,fl_progressive/https://www.wetterer.de/assets/images/responsive/popup/grillen/Texas-Ranger-Smoker-D71_0255.jpg" 
	data-sizes="auto"
	width="100vw"
    class="lazyload blur-up cld-responsive">

<img 
    data-src="//res.cloudinary.com/dsuwkv08y/image/fetch/q_auto,f_auto,w_auto,c_scale,fl_progressive/https://www.wetterer.de/assets/images/responsive/popup/grillen/Texas-Ranger-Smoker-D71_0256.jpg" 
	data-sizes="auto"
	width="100vw"
    class="lazyload blur-up cld-responsive">

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