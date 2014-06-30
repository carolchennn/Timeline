A Fork of Vertical Timeline
-----------------------------------------------------------
(This is a fork of WNYC's Super Awesome Vertical Timeline)

Check out the original README file at OriginalREADME.md.

A running example can be found [here](http://carolchennn.github.io/Timeline/).

## How to Use

### 1) Set up your data using Tabletop.js

Create a Google Spreadsheet with the following columns:
* title
* date
* display date
* photo url
* caption
* body 
* read more url
* class

**Please note that the _display date_ column must be in the format _Month day, Year_ (April 25, 2012) for proper javascript parsing.**
**Also, all columns must be _plain text_ format, including the two date columns.**
**Change the following items in html to custom the class, and if you don't like class, don't put that into your spreadsheet.**

 	(class "negative", for example, makes the post appear white on black)
 
 	.negative div.inner, .negative div, .negative h3 {
 		background: #000 !important;
 		color: #fff !important
 	} 


In Google Docs, go up to the File menu and pick Publish to the web. Fiddle with whatever you want, then click Start publishing. A URL will appear, something like https://docs.google.com/spreadsheet/pub?hl=en_US&hl=en_US&key=0AmYzu_s7QHsmdDNZUzRlYldnWTZCLXdrMXlYQzVxSFE&output=html

key: the part between key= and &

The Spreadsheet used in the example index.html file is at [https://docs.google.com/spreadsheet/ccc?key=0AhVQ7rH5MwaHdDA1ekNFU0d1Vm9lREdzN0tsd0czS3c&usp=drive_web#gid=0](https://docs.google.com/spreadsheet/ccc?key=0AhVQ7rH5MwaHdDA1ekNFU0d1Vm9lREdzN0tsd0czS3c&usp=drive_web#gid=0)

### 2) Insert the Spreadsheet key into script.js

Find your Spreadsheet key, and replace the sample key on line 3 of `js/script.js` with the key to your Spreadsheet. 

You also need to update the name of the spreadsheet 'sheet' that holds the data on line 4 of 'js/script.js'.

### 3) Enjoy!


## Credits

[Balance Media](http://www.builtbybalance.com) for the design and coding.

The following plugins/libraries are used:
[jQuery](http://jquery.com/), [Isotope](http://isotope.metafizzy.co), [Tabletop.js](http://github.com/jsoma/tabletop), [Handlebars.js](http://handlebarsjs.com/), [jQuery imagesLoaded plugin](http://github.com/desandro/imagesloaded), and [jQuery resize event](http://benalman.com/projects/jquery-resize-plugin/)

NOTE: All of the elements are free for non-commercial use. Commercial use of [Isotope](http://isotope.metafizzy.co) requires a $25 [license](http://metafizzy.co/#isotope-license).
