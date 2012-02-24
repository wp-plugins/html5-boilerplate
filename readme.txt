=== Plugin Name ===
Contributors: aarontgrogg
Tags: html5, boilerplate
Requires at least: 3.1
Tested up to: 3.3.1
Stable tag: 3.4

Based on the HTML5 Boilerplate created by Paul Irish and Divya Manian,
this allows for easy inclusion/removal of all HTML5 Boilerplate options.


== Description ==

Standing on the foreheads of giants (namely [Paul Irish](http://paulirish.com/)
and [Divya Manian](http://nimbupani.com/) and the good folks that have helped
them create and continue the growth of HTML5 Boilerplate, I present to you my
first WordPress plug-in, [HTML5 Boilerplate](http://html5boilerplate.com/).
As a spin-off of my [Boilerplate - Starkers WP Theme](http://aarontgrogg.com/boilerplate/),
this plug-in can be added to any theme, new, pre-existing, already customized, whatevs!

The clumsiest part of this plug-in is dealing with the CSS files.
To avoid any changes you make from being overwritten during upgrades,
"starter" files have been created in the plug-in's css directory.
I recommend copying the contents of the starter files into new files that you
can safely edit.  That way, if the starter files are updated later, you can
simply copy/paste from them into your files again, and all is fine.

Another route would be to add `@import` statements at the top of
your file, but this does increase your HTTP Requests, which hurts performance...
Your call, let me know if you can think of a better implementation.)

Cannot for the life of me figure out how to make the screenshots work in the `readme.txt`, so here are the links...

1. [screenshot-admin-screen.png](http://aarontgrogg.com/wp-content/plugins/html5-boilerplate/screenshot-admin-screen.png)
2. [screenshot-html-before.png](http://aarontgrogg.com/wp-content/plugins/html5-boilerplate/screenshot-html-before.png)
3. [screenshot-html-after.png](http://aarontgrogg.com/wp-content/plugins/html5-boilerplate/screenshot-html-after.png)

More about this plug-in can be found at:
[http://aarontgrogg.com/html5boilerplate/](http://aarontgrogg.com/html5boilerplate/)

I also built a Boilerplate theme based on [Elliot Jay Stocks'](http://elliotjaystocks.com/)
[Starkers Theme](http://starkerstheme.com/) that can be found at:
[http://aarontgrogg.com/boilerplate/](http://aarontgrogg.com/boilerplate/)

Please let me know if you have any questions/suggestions/thoughts,
Atg
[http://aarontgrogg.com/](http://aarontgrogg.com/)
[aarontgrogg@gmail.com](mailto:aarontgrogg@gmail.com)


== Installation ==

1. Download the ZIP
2. Unzip the ZIP
3. Copy/paste the unzipped files into your WP plug-in directory (`/wp-content/plugins/`)
4. From within WP's Plugin Admin panel, Activate the HTML5 Boilerplate plug-in
5. In the left-nav, within the Settings menu, you should now have an HTML5 Boilerplate link
6. Click the link to view the HTML5 Boilerplate Admin panel
7. Check and un-check options to add and remove stuff from your site!


== Frequently Asked Questions ==

= What HTML5 Boilerplate options does the plug-in let me manipulate? =
* Use HTML5 `DOCTYPE`?
* Add IE Conditional `<html>` Tags?
* Move XFN profile from `<head>` to `<link>`?
* Use HTML5 Character-Encoding `<meta>` Tag?
* Kill IE6 Image Toolbar?
* Force IE-edge / Google Chrome?
* Add Google Verification?
* Force iThings to Use Full Zoom?
* Add Favicon?
* Add iThing Favicon?
* Add IE-only CSS file?
* Add Modernizr JS?
* Add Respond JS?
* Add jQuery JS?
* Which jQuery version?
* Put jQuery in `<head>` or at end of `<body>`?
* Add jQuery Plug-ins JS?
* Add Site-specific JS?
* Add Google Analytics?
* Use HTML5 Search `<input>` Type?
* Add Search `placeholder` Text?
* Add Cache Buster to CSS &amp; JS Files?


== Screenshots ==

1. [screenshot-admin-screen.png](screenshot-admin-screen.png)
2. [screenshot-html-before.png](screenshot-html-before.png)
3. [screenshot-html-after.png](http://aarontgrogg.com/wp-content/plugins/html5-boilerplate/screenshot-html-after.png)


== Changelog ==

= 3.4 =
Missed a couple files...

= 3.3 =
2012-02-24:
* Converted `... />` to  `...>` for all the stuff this plug-in writes to the page.
* Updated `/css/style-starter.css` to latest HTML5 Boilerplate version.
* Updated jQuery to 1.7.1.
* Updated Modernizr to 2.5.3, Custom Build.
* Added 57x57 iThing favicon link.
* Fixed Bug introduced by WP 3.3+ that causes jQuery to be loaded after site-specific JS.

= 3.2 =
2011-06-09:
Was still calling jQuery 1.5.1, erps!  Not only fixed that, but now allow users to enter version number, so they can upgrade when they want.  Thanks, Micah.
Line 522 had the wrong function comment.  Thanks, Micah.
Added option of putting jQuery/plug-ins in the `<head>` to make it more compatible with more plugins.  Thanks, Micah.
Fixed `ob_end_flush()` issues with some themes.  Thanks, Chris!
Improved `DOCTYPE`, `<html>` and `<head>` filtering to cover various versions.

= 3.1 =
2011-06-09:
Attempting to fix a few odd text appearances.

= 3.0 =
2011-06-01:
Bumping-up revisions a whole knotch, as quite a few changes here...
* Fixed typo on Admin panel (removing trailing `/` in HTML5 doctype), thanks @paul_irish.
* Per Paul & Divya recommendations:
	- Dropping cdnjs link for Modernizr, resorting to local link only, hopefully soon that will be replaced with Google CDN link.
	- Removed handheld.css, because "our research has shown not enough devices read it to make it worthwhile". Additionally, if you're doing your CSS right (a la Responsive Design, you're building for smaller screens first, then adding CSS for larger screens via `@media` queries, right?).
	- Removed print.css because "extra print stylesheets are downloaded at load, so its a big hit"; this, too, is best served via `@media` queries in your main CSS.
	- Removed YUI Profiling stuff because you "probably weren't using it anyway", right?
	- Removed Belated PNG because it "is a really slow solution and an overkill for PNGs", check [http://html5boilerplate.com/docs/#Notes-on-using-PNG](http://html5boilerplate.com/docs/#Notes-on-using-PNG) for deets on dealing with PNGs in ye olde IE.
* Added removal of IE6 Image Toolbar to Admin panel.
* Added iPad and iPhone 4 favicon links to existing "iThing Favicon" block.
* Added [Respond.js](http://filamentgroup.com/lab/respondjs_fast_css3_media_queries_for_internet_explorer_6_8_and_more/) option to Admin panel.
* Added [Google Verification](http://www.google.com/support/webmasters/bin/answer.py?answer=35179) option to Admin panel.
* Updated `/css/style-starter.css` to latest HTML5 Boilerplate version.
* Updated jQuery to 1.6.1.
* Updated `/js/plugins.js` to include `console.log` bit.

= 2.2 =
2011-05-11:
Added features to move XFN Profile link, convert Search input type to "search", add custom placeholder text, and add cache buster to all CSS/JS URLs.
Phew!

= 2.1 =
2011-05-10:
Forgot the `/` between `BP_PLUGIN_URL` and the rest of the URL... erps!  Also did a little clean-up on how the Google Analytics gets applied.
Lastly, giving the screenshots one... last... try...

= 2.0 =
2011-05-10:
Finally found [an article](http://wordpress.org/support/topic/updated-my-plugin-listing-still-showing-old-version?replies=7) that tells me that
not only do I need to update the "Stable tag" in the `readme.txt` and copy all the plug-in files to a new `Tag` folder, but also the `Version` in the plug-in
file itself... So, hopefully this will finally get the latest plug-in into the Repository...  :-)

= 1.3 =
2011-05-08:
Updating jQuery version to 1.6 and hopefully fixing links on Screenshot page.

= 1.2 =
2011-04-25:
Reviewing additional HTML5 Boilerplate pages, adding [Google Fix URL option](http://www.google.com/support/webmasters/bin/answer.py?answer=136085)
to HTML5 Boilerplate Admin panel.

= 1.1 =
2011-04-24:
Trying to get Screenshot links working in `readme.txt`...
May or may not work...  :-)

= 1.0 =
2011-04-21:
Well, this is the first version, so... here it is!  This version includes
all of the nutritious goodness from HTML5 Boilerplate as of April 21, 2011.
