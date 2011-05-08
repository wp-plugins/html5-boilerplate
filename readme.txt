=== Plugin Name ===
Contributors: aarontgrogg
Tags: html5, boilerplate
Requires at least: 3.1
Tested up to: 3.1.1
Stable tag: 1.3

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
* Use HTML5 DOCTYPE
* IE Conditional Tag
* Replace old-school, long-hand character-encoding `<meta>` with HTML5-version
* Google Chrome / IE-edge
* iThings use full zoom
* Add Favicon
* Add iThing Favicon
* IE CSS
* Handheld CSS
* Print CSS
* Modernizr JS
* jQuery JS
* jQuery Plug-ins JS
* Site-specific JS
* Yahoo! Profiling JS
* Belated PNG JS
* Google Analytics


== Screenshots ==

1. [Screen shot of Settings > HTML5 Boilerplate link & Admin screen](http://aarontgrogg.com/html5boilerplate/files/2011/04/screenshot-admin-screen.png)

2. [View Source before HTML5 Boilerplate](http://aarontgrogg.com/html5boilerplate/files/2011/04/screenshot-html-before.png)

3. [View Source after HTML5 Boilerplate](http://aarontgrogg.com/html5boilerplate/files/2011/04/screenshot-html-after.png)


== Changelog ==

= 1.3 =
2011-05-08: Updating jQuery version to 1.6 and hopefully fixing links on Screenshot page.

= 1.2 =
2011-04-25: Reviewing additional HTML5 Boilerplate pages, adding [Google Fix URL option](http://www.google.com/support/webmasters/bin/answer.py?answer=136085)
to HTML5 Boilerplate Admin panel.

= 1.1 =
2011-04-24: Trying to get Screenshot links working in readme.txt...
May or may not work...  :-)

= 1.0 =
2011-04-21: Well, this is the first version, so... here it is!  This version includes
all of the nutritious goodness from HTML5 Boilerplate as of April 21, 2011.
