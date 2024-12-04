---
title : "WordPress 2.9: errors in class-json.php, lines 115 and 238?"
author : "Niklas"
date : "2009-12-30"
categories : 
 - tech
 - wordpress
---

[![Computer says no.](http://farm1.static.flickr.com/106/287571800_69ff9a91eb_m.jpg "Computer says no.")](http://www.flickr.com/photos/44124300615@N01/287571800)

Image by [Niklas](http://www.flickr.com/photos/44124300615@N01/287571800) via Flickr

If you're wondering why your spanking new [WordPress](http://en.wikipedia.org/wiki/WordPress "WordPress") 2.9 upgrade/install brings you the following line everywhere:

> `Fatal error: Cannot redeclare class services_json in /wp-includes/class-json.php on line 115`

...it's because [Alex King](http://alexking.org/ "Alex King")'s otherwise sweet plugin [Twitter Tools](http://alexking.org/projects/wordpress) generates it. Deactivate the plugin and you're OK. It didn't actually do anything bad for me except mess with my sidebar plus adding the above line in every single page in the admin interface.

I'm sure Monsignieur King will fix this quite soon.

Then, another bit gave me the following error message, popping up to and fro, both in my blog and in the admin interface:

> `Warning: Cannot modify header information - headers already sent in /wp-includes/class-json.php on line 238`

This one was because of the Intense Debate plugin, which I found [thanks to vermontjohn and alism in the WordPress forums](http://wordpress.org/support/topic/346425). I'm using the most current version (2.5) and still the problem pops up. I've sent the developers a complete error description and will be awaiting a reply.

**update 1, 2009-12-30, 20:47**: I've received an e-mail from one of the developers of Intense Debate:

> Hi Niklas,
> 
> Thanks for getting in contact. We're taking a look and will have some news shortly.
> 
> Thanks, Michael
