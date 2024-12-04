---
title : "WordPress 2.1 hits like a frikkin’ rock"
author : "Niklas"
date : "2007-01-22"
categories : 
 - heroes
 - tech
 - wordpress
---

[WordPress](http://wordpress.org), the best blogging platform in the world, [has gone v2.1](http://wordpress.org/development/2007/01/ella-21) which means [a bunch of things](http://www.technosailor.com/10-things-you-should-know-about-wordpress-21).

So, any problems upgrading for me? Not really, apart from luckily noticing that I had to overwrite `wp-cache.php`; I was getting bizarre error-messages before that, relating to [WP-Cache](http://mnm.uib.es/gallir/wp-cache-2), saying the following:

`Call to undefined function: add_filter() in /home/[my_home_dir_name]/public_html/wp-includes/default-filters.php on line 4`

...but after overwriting `wp-settings`.php, everything was healthy. After that I just had to run the upgrade-script and sing a merry song with the people at [the WordPress IRC Live Help channel](http://codex.wordpress.org/IRC).

Thanks a lot for the release!

My first impressions:

- I love the fact that WP now automatically saves drafts of posts. Mind you - "The title of the post must be filled out in order for autosaving to occur."
- The Dashboard looks uglier: the fonts that display news are bigger and uglier.
- The Dashboard is faster than v2.0.7: this also goes for a lot of the other pages in WP.
- I'd like to delete the new, second default category "other blogs"; I'd at least like to be able to rename it.
- [The upgrade section of the WordPress site](http://codex.wordpress.org/Upgrading_WordPress) is rarely in sync with a newly released version of WP. Could be I'm just a geek waiting for the minute something new drops, but whaddaell!
- Links are now called "Blogroll", and the description one applies in this list is no longer visible in the sidebar; not in mine anyway.
