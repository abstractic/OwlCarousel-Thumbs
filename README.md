# Owl Carousel 2 (thumbnails plugin)
This is a modified version of [GijsRoge](https://github.com/gijsroge/OwlCarousel2-Thumbs) JavaScript library to add thumbnail support for Owl Carousel 2.0.

## Quick notes
This plugin has been modified to support as many photos as you like in your gallery and thumbnails that do not fit within the boundaries of your gallery will be hidden until its closest sibling is clicked and highlighted.

Thumbnails will behave as your photos and only a few of your thumbnails will be visible at a time. To allow this behaviour, the only difference of this modified plugin is that it contains an extra HTML wrapper around your thumbnail items.

## Quick start
Download the [latest release](https://github.com/abstractic/owl-carousel-thumbs.git) of this plugin and add it to your JavaScript files bundle behind the default Owl Carousel 2.0 library.

#### Simple setup
```javascript
$(document).ready(function() {

	$('.owl-carousel').owlCarousel({
		
		thumbs: true
	});
});
```

## HTML setup
This plugin can generate your thumbnails automatically, but by default this plugin is setup to look for your HTML output as described below.

```html
<div class="owl-carousel" data-slider-id="1">
	<div>[your image]</div>
	<div>[your image]</div>
	<div>[your image]</div>
	<div>[your image]</div>
</div>
<div class="owl-thumbs" data-slider-id="1">
	<div class="owl-thumbs-wrapper">
		<button class="owl-thumb-item">[your image thumbnail]</button>
		<button class="owl-thumb-item">[your image thumbnail]</button>
		<button class="owl-thumb-item">[your image thumbnail]</button>
		<button class="owl-thumb-item">[your image thumbnail]</button>
	</div>	
</div>
```

## Available options
There are a few plugin options that can be used to control the HTML output of your image gallery:

1. **thumbs** - this option enables the thumbnails on your gallery.
2. **thumbImage** - enable this option if you want this plugin to generate the thumbnails for you.
3. **thumbsPrerendered** - disable this option if you want this plugin to generate the thumbnails for you.
4. **thumbContainerClass** - this option controls the class name of your thumbnail container (must match your pre-rendered HTML).
5. **thumbWrapperClass** - this option controls the class name of your thumbnails wrapper (must match your pre-rendered HTML).
6. **thumbItemClass** - this option controls the class name of your thumbnail items (must your pre-rendered HTML).

To override the default plugin options, just add them to your carousel init function.

```javascript
$(document).ready(function() {

	$('.owl-carousel').owlCarousel({
		
		thumbs: true,
        thumbImage: false,
        thumbsPrerendered: true,
        thumbContainerClass: 'owl-thumbs',
        thumbWrapperClass: 'owl-thumbs-wrapper',
        thumbItemClass: 'owl-thumb-item'
	});
});
```

## Demo
A demo is coming, sadly been too busy with current project :)
