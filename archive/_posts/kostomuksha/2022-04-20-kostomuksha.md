---
layout: post
title:  "Карелия. Костомукша (Посетить)"
date:   2022-04-20 18:38:00 +0300
tags: [Путешествие, Посетить]
---
*Город в республике Карелия, построенный финами*

<style type="text/css">
.wrapper {
  max-width: 890px !important;
}
</style>
<main class="gallery">
	<div class="grid-sizer"></div>
	{% for img in site.data.gallery.kostomuksha.urls %}
	<div class="grid-item">
		<a href="{{img}}" data-fslightbox><img src="/assets/img/transparent.gif" data-original="{{img}}" alt="{{site.data.gallery.kostomuksha.alt}}"></a>
	</div>
	{% endfor %}
</main>
<script src="https://ajax.googleapis.com/ajax/libs/jquery/3.6.0/jquery.min.js"></script>
<script src="/assets/js/jquery.lazyload.js"></script>
<script src="/assets/js/masonry.pkgd.js"></script>
<script src="/assets/js/fslightbox.js"></script>

<script>
	var images = $('img');
	var grid = $('main.gallery');

	grid.masonry({
		itemSelector: '.grid-item',
		columnWindth: '.grid-sizer',
		gutter: 5,
		percentPosition: true
	});

	images.lazyload({
		effect: "fadeIn",
		effectTime: 1000,
		threshold: 0,
		delay: 5000,
		load: function () {
			grid.masonry('layout');
		}
	});
</script>
