---
title: "Responsible Image Test"
date: 2020-01-19T10:38:25+01:00
categories: [Responsive Design]
---


Test von responsible Images

<!--more-->

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
    class="lazyload blur-up cld-responsive" />

<img 
    data-src="//res.cloudinary.com/dsuwkv08y/image/fetch/q_auto,f_auto,w_auto,c_scale,fl_progressive/https://www.wetterer.de/assets/images/responsive/popup/grillen/Texas-Ranger-Smoker-D71_0252.jpg" 
	data-sizes="auto"
    class="lazyload blur-up cld-responsive" />

<img 
    data-src="//res.cloudinary.com/dsuwkv08y/image/fetch/q_auto,f_auto,w_auto,c_scale,fl_progressive/https://www.wetterer.de/assets/images/responsive/popup/grillen/Texas-Ranger-Smoker-D71_0253.jpg" 
	data-sizes="auto"
	width="100vw"
    class="lazyload blur-up cld-responsive" />
<img 
    data-src="//res.cloudinary.com/dsuwkv08y/image/fetch/q_auto,f_auto,w_auto,c_scale,fl_progressive/https://www.wetterer.de/assets/images/responsive/popup/grillen/Texas-Ranger-Smoker-D71_0254.jpg" 
	data-sizes="auto"
	width="100vw"
    class="lazyload blur-up cld-responsive" />

<img 
    data-src="//res.cloudinary.com/dsuwkv08y/image/fetch/q_auto,f_auto,w_auto,c_scale,fl_progressive/https://www.wetterer.de/assets/images/responsive/popup/grillen/Texas-Ranger-Smoker-D71_0255.jpg" 
	data-sizes="auto"
	width="100vw"
    class="lazyload blur-up cld-responsive" />

<img 
    data-src="//res.cloudinary.com/dsuwkv08y/image/fetch/q_auto,f_auto,w_auto,c_scale,fl_progressive/https://www.wetterer.de/assets/images/responsive/popup/grillen/Texas-Ranger-Smoker-D71_0256.jpg" 
	data-sizes="auto"
	width="100vw"
    class="lazyload blur-up cld-responsive" />

{% include _references.md %}
