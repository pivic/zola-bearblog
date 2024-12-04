---
title : "Techy tips, mostly on WordPress"
author : "Niklas"
date : "2005-12-30"
categories : 
 - tech
---

As [WordPress 2.0](http://wordpress.org) is starting to roll out, some interesting plugins have started to show up, already.

My favourite newbie is [Picture Frame](http://www.paulchiu.net/projects/picture-frame) by Paul Chiu. As you've probably noticed, I've started posting pictures again. Well, only three so far, using this plugin. It allows a user to quickly and gently opt to display a picture in a frame, and that frame can be created by yourself. Check out said link for the plugin. A techy note on this, is that I couldn't get it to work from the get-go, but after a very quick e-mail response from Paul, where he suggested I changed

`$pf_setting['frame_default'] = "pictureFrame";`

to

`$pf_setting['frame_default'] = "pictureFrame.gif";`

...and it's worked without a hitch since then. Now, before you happily implement this in your system, please bear in mind, that if Paul one day should decide to scrap said plugin, WordPress evolves and the plugin doesn't work after an upgrade - you're fawked. In other words, if you find yourself in that situation, you'd better quickly find 1) a programmer that can get the plugin working again or 2) some time over to manually edit your pictures so they don't wind up 3000\*5000 in your posts.

I really like Ozh's "[Wordpress Admin Drop Down Menu](http://frenchfragfactory.net/ozh/my-projects/wordpress-admin-menu-drop-down-css TARGET=)" that's really just good for us lazy admins who dislike clicking more than necessary. Only for WordPress 2.0.

I'm keen on the [Audio Player](http://www.1pixelout.net/code/audio-player-wordpress-plugin) that's popped up as well. Note I haven't tried it, and it's made to play snippets of music, but it buffers and displays the name of the artist along with the title, so that's nice.

I've neither tried [WordPress Flickr Post Bar](http://tantannoodles.com/toolkit/wp-flickr-post-bar), and even though it's not certified for WordPress 2.0 (if you have the WYSIWYG editor enabled, but the author says a change is "forthcoming", whenever that may be) it's interesting anyway, and promises integration with [FAlbum](http://www.randombyte.net/blog/projects/falbum), one of my favourite plugins for WordPress: it lets you configure a flickr-page of your own, like [this page](https://niklasblog.com/wp-content/plugins/falbum/wp/album.php) that's part of my blog. Brilliant plugin, very aesthetic. Speaking of flickr, [here](http://pchere.blogspot.com/2005/03/great-flickr-tools-collection.html)'s an enormous list of _a lot_ of flickr tools.

**edit**: I just found out about [WP Tiger Administration](http://orderedlist.com/wordpress-plugins/wp-tiger-administration), which turns your admin interface into [something from OSX Tiger](http://frenchfragfactory.net/ozh/images/wordpress_adminmenu_tiger.gif).

That's it about WordPress, now for two other nerd droplets. If you need a freeware DVD-ripper for Windows, check out [StaxRip](http://www.planetdvb.net/staxrip/download.htm). Yeah, the author's a soul fan. Also, some of [the PowerToys for Windows](http://www.microsoft.com/windowsxp/downloads/powertoys/xppowertoys.mspx) are great, especially if you're running Windows XP.
