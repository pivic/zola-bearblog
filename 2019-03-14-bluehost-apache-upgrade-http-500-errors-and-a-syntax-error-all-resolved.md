---
title : "BlueHost, Apache upgrade, HTTP 500 errors, and a syntax error: all resolved"
author : "Niklas"
date : "2019-03-14"
categories : 
 - materialism
 - tech
 - wordpress
---

![](https://niklasblog.com/wp-content/Screenshot-2019-03-14-at-16.21.28.jpg)

About 18 hours ago, I received this e-mail from BlueHost, which is the company that currently hosts this blog:

\[...\] we’re excited to announce that we will be upgrading all of our servers to newer versions of Apache and providing newer versions PHP (including PHP 7.1 & 7.2). The upgraded versions provide better data processing, which can improve the performance and speed of your website.  
  
**When will maintenance begin?** We will start the maintenance process on March 13 at 6 PM EST and will continually monitor your website. We anticipate less than 5 minutes of slowness/downtime during the upgrade itself.

As I like to live life dangerously (as a white, middle-aged man like myself says), I run beta or alpha versions of WordPress. As such, I contacted BlueHost back in December (of 2018) and asked them to upgrade my PHP version to at least 7.3. They did; I subsequently upgraded WordPress some more, and no issues.

Until today, after BlueHost upgraded Apache and possibly downgraded my PHP version as well; I'm not sure about the latter, but hang in there.

I noticed that my WordPress site was down, as it threw an [HTTP 500 Error](https://www.lifewire.com/500-internal-server-error-explained-2622938) as I tried to access the main page; access to individual pages was also impossible.

After BlueHost upgraded, this appeared when I checked out individual pages—while the main blog page just gave a HTTP 500 Error:

```
Parse error: syntax error, unexpected '[' in /var/www/my_wp_path/wp-content/plugins/block-gallery/includes/admin/class-block-gallery-action-links.php on line 87.
```

That error is detailed here:

https://github.com/thatplugincompany/block-gallery/issues/20

However, BlueHost resolved the entire matter by (they claim):

1. upgrading PHP
2. renaming php.ini

The weird thing is that my cPanel in BlueHost claims that I'm currently using **PHP 5.6.40**. Still, WordPress is (not yet) complaining about it, and everything is back to normal; no slowness issues or anything like that so far.
