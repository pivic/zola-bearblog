---
title : "A few things to keep in mind when upgrading to WordPress 3.5 + personal experience from upgrading from 3.2.1 to 3.5.1"
author : "Niklas"
date : "2013-04-04"
categories : 
 - tech
 - wordpress
---

First of all: I've used [**WordPress**](http://wordpress.org) for ages and I love it. No problems there.

Their [requirements page](http://wordpress.org/about/requirements) states stuff clearly, as well as what you need to [consider before upgrading](http://codex.wordpress.org/Updating_WordPress).

On the other hand, there are other issues.

The number one thing you should do: **document the entire installation/upgrade process**. Don't rely on memory. Passwords need to be safely stored, customisations made will have to be remembered (unless you're prepared to face hell for the forgotten customisations come the next upgrade), if you make any oddball changes to files, make sure you keep a version backup history and a documentation of it, so that you don't end up with "which files are these?" in a few months, only to delete them and cry later.

Second, **make sure your host is ready for an upgrade**. _Really_, make sure. Ask them. Don't take their "we provide the following, we promise" page for granted. Ask them. I'll clarify why this is import a bit later.

Then, **make sure your WordPress theme works with 3.5**. Download [Instant WordPress](http://www.instantwp.com) and go from there. Take the time required to delve into all of your customisations (if you're upgrading), not only in the theme but in the code as well (if you've configured it manually). There are things in themes that can, and often will break, if you simply upgrade to 3.5.1 without caring.

**Backup everything**. Files, the database: the works. My hosting provider, BlueHost, actually only offer restores as a _[courtesy](https://my.bluehost.com/cgi/help/312)_. Think about what that truly means.

**If you're not technically savvy: ask a techy friend before upgrading**. Seriously, do just that. I asked [Naoko](http://en.naoko.cc) about my theme - the great Orange Sky - and pestered her to bits, asking if she could consider upgrading it. And she did. I actually tried upgrading my blog one time before she fixed the theme - which resulted in my restoring the WordPress database and additional files to boot.

**Check with your host that the coming upgrade is OK to perform**. When I hit problems as I upgraded from 3.2.1 to 3.5.1, my host, BlueHost, actually came up with some really weird, truly stupid and also erroneous responses. I upgraded using their technology - [SimpleScripts](http://www.simplescripts.com) - which ended up with SimpleScripts saying "Your upgrade is complete!" while the first page of my blog complained that their MySQL version was below 5.0, which is the minimum requirement to run WordPress 3.5. This is what I meant when I earlier wrote about really checking that your host is _really_ ready for WordPress 3.5. When I lodged a support ticket about this, the reply was a boilerplate "You can change your PHP version here" response. Well, if only the error message had been about PHP... I then chatted with them, and they were like "You have more than 200 000 files in your database!" to which I had to reply that no, there are no files in the database; are you referring to the number of rows? "Yes". Well, no; that's not a limit according to [your TOS](http://www.bluehost.com/terms_of_service.html). Great Scott.

The fun didn't stop there. BlueHost tried to chat with me for _an hour_ about the problem I had, not really asking good questions, and I said I had to leave but would like to continue the conversation over e-mail. No response. But wait - my blog was upgraded! Wee! While they didn't contact me after that, the blog was upgraded - apart from one thing. The character set/collation had been completely fucked up. Swedish letters and other "odd" characters produced junk letters. So I chatted with another BlueHost person who was quick to say that yes, we helped you, and yes, that's your problem despite us doing it to you. ((I wonder how BlueHost would react in a trial, if the company were human and accused of rape.))

Instead of chatting further about that - which felt like swimming against a very hard stream, designed to kill me - I fixed the problem myself, using the free WordPress plugin named [Search and Replace](http://wordpress.org/extend/plugins/search-and-replace). Using it, you just pop in an erroneous character and tell the plugin what you want to replace it with. Presto. All fixed.

**Upgrade**. Preferably using [the automatic built-in upgrade process from within WordPress](http://codex.wordpress.org/Updating_WordPress#Automatic_Update) ((Valid from WordPress 2.7 and onwards.)); the Dashboard will alert you to any available upgrades. Do this with the tech savvy person you know so well if you need to (if you feel you don't know or don't have all bases covered - _find that friend_). If you do a manual upgrade, check [the WordPress list regarding that](http://codex.wordpress.org/Updating_WordPress#Manual_Update).

When done, check your blog for errors. Is everything looking good? Widgets are in the right places? Are the plugins working as expected? No weird characters anywhere?

Now, I'm happy. I'm able to use [Jetpack](http://wordpress.org/extend/plugins/jetpack)! Everything doesn't take ages to load (which often is the case, using old technology).

Do what [ITIL](http://en.wikipedia.org/wiki/Information_Technology_Infrastructure_Library) refers to as [CSI](http://wiki.en.it-processmaps.com/index.php/ITIL_V3_CSI_-_Continual_Service_Improvement): go through the list that you made first, and then see what was actually done, if it can be done better next time, if there's something that needs to be added to or removed from the list.
