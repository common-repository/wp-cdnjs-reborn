=== WP CDNjs Reborn ===
Contributors: audioscavenger, mindshare, geetjacobs, patkirts
Tags: CDNjs, cloudflare, js, css, scripts, cdn, libraries
Requires at least: 5.1
Tested up to: 5.2
Stable tag: 0.3.3
License: GPLv3 or later
License URI: https://www.gnu.org/licenses/gpl.html

Integrates easily CSS and JavaScript Libraries hosted by CDNjs.com. Browse, select version and sub-assets to fit your needs.

== Description ==

Speed up your site by using the powerfull and free CDNjs. This plugin Allows you to search all http://cdnjs.com libraries and include them on your site.
Proudly served by [Audioscavenger](http://www.blog.derewonko.com/).

/!\ This is a fork from WP cdnjs by Mindshare Labs, which have merged since 0.3.0. I keep both projects up to date and they are now exactly the same. Maybe this one will disappear one day since both are the same and 100% compatibles.


**Requires PHP 5.3 or newer**
![Tested in WordPress](https://img.shields.io/wordpress/v/akismet.svg) ![PHP 5.3+](https://img.shields.io/badge/PHP-5.3%2B-blue.svg) ![jQuery](https://img.shields.io/badge/jQuery-1.11.4-ff69b4.svg) ![Bootstrap](https://img.shields.io/badge/Bootstrap-3.3.x-6f5499.svg)

= Browse by Name and Description =
When browsing, the search key word look in the library names and description.

* Shows library name
* Shows description
* Shows how many versions are available

= Choose the Righ Version =
Stop worrying about incompatibilities, WP CDNjs Reborn let you chose the version you really need!

* Latest version selected by default
* Minified version selected by default
* Allows you to include the (non)minified version for debugging purposes

= Add More Assets =
Among the libraries served by CDNjs, you can add the assets related.

* Shows all the assets associated with a library version
* Allows you to change the main asset used
* Allows you to add and remove assets
* Shows the assets already used in grey to avoid addind duplicates

= Manage Priorities =
With an easy drag&drop, manage the order in which your libraries will be loaded.

* Easy drag&drop
* Header/Footer choice
* Enable/Disable option


== Installation ==

Upload the plugin to your blog or install it via the dashboard, activate it, done.
The configuration page is found under Settings->WP CDNjs Reborn

This plugin requires PHP and JavaScript.


== Frequently Asked Questions ==

= Is WP CDNjs Reborn Free? =
Yes! Every WP CDNjs Reborn's features are and always will be free.

= Do I need a WordPress.com account? =

Since WP CDNjs Reborn do not provided hosted services by WordPress.com, a WordPress.com account is not required.

= How do I contribute to WP CDNjs Reborn? =

There are opportunities for developers at all levels to contribute.
You can clone the [WP CDNjs Reborn Git](https://github.com/audioscavenger/wp-cdnjs-reborn) and pull requests from here.

= How can I change what action is used to enqueue the CDNJS scripts? =

You can override the default action ('init') that enqueues the CDNJS script like so:
`
add_filter('wp_cdnjs_init_action', 'my_cdnjs_init_action');
function my_cdnjs_init_action() {
	return 'get_sidebar'; // the action tag you wish to use
}
`

= Is it possible to have all enabled scripts load in the WordPress Admin area? =

Yes. You can use this filter:
`
add_filter('wp_cdnjs_allow_in_admin', 'my_cdnjs_allow_in_admin');
function my_cdnjs_allow_in_admin() {
	return TRUE;
}
`


== Screenshots ==

1. Dashboard: Set of libraries and usual messages.
2. Dashboard: Browse cdnjs Libraries example with popup.
3. Dashboard: Browse available versions for twitter-bootstrap.
4. Dashboard: Browse available assets for twitter-bootstrap.


== Changelog ==

= 0.3.3 =

**Minor Update**
* just tested for 5.2
* Minimum version required at least 5.1 to force you guys update core engine. Security matters.
* tested with both PHP 7.0 and 7.2.18

= 0.3.2 =

**Minor Update**
* just tested for 5.1.1
* Minimum version required at least 5.0 to force you guys update core engine. Security matters.

= 0.3.1 =

**Minor Update**
* just tested for 4.9.6 + updated EOL of main script
* Minimum version required at least 4.9 to force you guys update core engine. Security matters.

= 0.3.0 =

**Major Enhancements**
* Performance increase: Removed the query strings everywhere
* Removed font-awsome and switched to WP dashicons

= 0.2.4 =

**Bug Fix**
* Correct path to language files + add en_US.mo

= 0.2.3 =

**Enhancements**
* Ajout de la version Francaise, vieux.

= 0.2.2 =

* Release date: January 7, 2018
* Release post: [WP CDNjs Reborn](https://wp.me/p9sB0t-7Y)

**Enhancements**
* Creation of the readme.txt. This took me like 3 hours so it totally justifies a new release.

= 0.2.1 =

**Major Enhancements**
* add menu_icon + css assets
* rename wp-cdnjs.php to wp-cdnjs-reborn.php
* integrate 0.13 functions
* move main functions to lib/functions.php
* add minified js
* table in Settings is now full width
* cleanup php code everywhere

= 0.2.0 =

**Major Enhancements**
* Initial fork from [wp-cdnjs.git](https://github.com/mindsharelabs/wp-cdnjs.git) to [wp-cdnjs-reborn.git](https://github.com/audioscavenger/wp-cdnjs-reborn.git)
* Fix the secondary assets you want to include
* Add column for choosing the exact version
* Add checkbox for choosing the the non-minified version

