---
title : "Pinebook Pro: my review (July 2020)"
author : "Niklas"
date : "2020-07-15"
categories : 
 - culture
 - heroes
 - linux
 - materialism
 - tech
 - video
---

![](https://niklasblog.com/wp-content/pinebookpro.jpg)

?????

Table Of Contents

- [First impressions](#first-impressions)
- [First small tweaks](#first-small-tweaks)
- [Installing software](#installing-software)

- [Running other operating systems from an SD card](#running-other-operating-systems-from-an-sd-card)
- [Sync](#sync)
- [Obsidian (or, rather, not)](#obsidian-or-rather-not)
- [Markdown editor](#markdown-editor)

- [Remarkable](#remarkable)
- [Kate](#kate)

- [Viewing: Okular or Evince](#viewing-okular-or-evince)
- [Shell](#shell)
- [Process viewer](#process-viewer)
- [KDE Connect](#kde-connect)
- [Netflix](#netflix)
- [Using video via USB-C](#using-video-via-usb-c)
- [Performance tricks](#performance-tricks)

- [Swapping](#swapping)
- [Processor tweaking](#processor-tweaking)

- [Issues](#issues)

- [Keyboard settings](#keyboard-settings)
- [High-pitched (yet quiet) noise from the laptop](#high-pitched-yet-quiet-noise-from-the-laptop)
- [Trackpad](#trackpad)

- [Summary](#summary)

I just received my [Pinebook Pro](https://www.pine64.org/pinebook-pro/).

It's a laptop that costs 200 USD to purchase. It's manufactured by an organisation, PINE64, who want to deliver community-driven stuff. They make laptops, stationary computers, a phone, and a wristwatch, which are all—except for the watch—running Linux. Or, actually, any operating system that handles the processor architecture: you're free to choose whatever you'd like to use.

PINE64 have [a philosophy](https://www.pine64.org/philosophy/) stated, a highly-transparent [wiki](https://wiki.pine64.org/index.php/Main_Page), a very helpful community, and loads of partnerships with other organisations and companies that create exciting stuff. They're also very transparent with issues that their products have and provide actual resolutions (do you hear me, Apple, et al?). I'll get back to that last bit later.

Every bit of hardware is documented and made with tinkerers in mind. You want to swap the memory for something else? Just order it from them. You want to open the device and replace something? There's documentation for it, so go right ahead. Install which ARM-compatible operating system you like. Nothing is bloated with malware. Nothing is spying on you. You can contribute to most of the software that you'd like to install.

![](https://niklasblog.com/wp-content/image-44.png)

Every little thing is open. You get to see what's inside. You can take out things, replace them with stuff that you prefer, even. This cannot be said for most other manufacturers.

* * *

To me, running Linux is a bit like listening to [this video](https://www.youtube.com/watch?v=mPZkdNFkNps) when you're at your most stressed.

The processor architecture is [ARM](https://en.wikipedia.org/wiki/ARM_architecture), which means that it is different from what Intel delivers. [This blog post](https://www.androidauthority.com/arm-vs-x86-key-differences-explained-568718/) contains extensive information on the subject, but let's just say I don't like the idea of there being backdoors into Intel's stuff. By the way, Apple are moving from Intel to building their own Arm-based processors.

* * *

Did I encounter issues? Yes, I did. I'll get to that in a bit, but I'm going to convey what happened when I installed my operating system in steps.

Pinebook Pro now comes pre-loaded with [Manjaro](https://manjaro.org/) and [KDE Plasma](https://kde.org/plasma-desktop) as my [desktop environment](https://en.wikipedia.org/wiki/Desktop_environment). This [distribution](https://en.wikipedia.org/wiki/Linux_distribution)—a Linux term that means a _Linux flavour_, much like different kinds of ice-cream—is very user friendly. I've been pleasantly surprised with everything in Manjaro so far, and please bear in mind that I'm mainly coming from a Windows and macOS background.

<iframe sandbox="allow-same-origin allow-scripts" src="https://peertube.mastodon.host/videos/embed/67d5c560-2002-498e-91af-433147fe2ab5" allowfullscreen width="560" height="315" frameborder="0"></iframe>

# First impressions

![](https://www.pine64.org/wp-content/uploads/2019/07/Pinebook_July.png)

The first thing I noticed when I received the laptop is that it's **lighter than I expected it to be**. I've used a bunch of different laptops, everything from heavy 1980s IBM machines to my current work laptop, a 13-inch, 2018-year-edition Apple MacBook Pro.

The second thing is that the machine is **unscathed by branding**. The only thing that reveals that this machine is made by PINE64 is an identifying sticker underneath the computer and a keyboard key that carries the emblem of a pine cone.

The third thing I noticed was how **sleek the introductory phase** was. I turned on the computer and there's, first of all, no noise; the laptop is fanless.

**The screen is big**. To me, it feels far more well made than many laptops that I've seen. Sure, technology is advancing, but this is 1920\*1080 resolution and altogether, for 200 USD, this is brilliant value for money (in a capitalistic society).

The Manjaro installation process is very simple and shows how things evolve in the PINE64 universe; Blog posts that are written in January 2020 about the setup process can be outdated. An example of this is that I didn't need to change root user name/password as the installation process takes care of this.

Finally, **the battery lasts a long time**. People state it lasts for 6-8 hours (depending on how it's used). I've yet to complain.

> The battery life wasn't as amazing as I hoped, but it wasn't bad, either—the battery discharged 18 percent over the course of an hour of full-screen [YouTube](https://www.youtube.com/watch?v=AgpWX18dby4) at 1080p. This isn't quite as good as the vastly more expensive HP Dragonfly Elite's 16-percent discharge, but it's far better than the (also vastly more expensive) Dell XPS 13 Developer Edition's 24-percent discharge in the same time frame. It's unclear what impact—negative _or_ positive—this unit's deranged LCD display may have had on the test.
> 
> Finally, the onboard 64GiB eMMC storage seems solid. I did the usual battery of fio testing on it, and it brings an average 1MiB write throughput just under 90MiB/sec, 4KiB sync write throughput of 2.1MiB/sec, and average 4KiB write latency of 0.1ms, with 99.99th percentile write latency of 2.4ms. It won't win any races with mid- to high-end "real" SSDs, but it's a solid performer unlikely to frustrate anyone for desktop use cases.
> 
> @arstechnica [https://arstechnica.com/gadgets/2020/06/pinebook-pro-review-a-200-foss-to-the-hilt-magnesium-chassis-laptop/](https://arstechnica.com/gadgets/2020/06/pinebook-pro-review-a-200-foss-to-the-hilt-magnesium-chassis-laptop/)

<script note="" src="https://cdn.jsdelivr.net/gh/Blogger-Peer-Review/quotebacks@1/quoteback.js"></script>

> With my smartphone having more processing power and memory than this laptop, it is no wonder that it’s pretty green and efficient. It uses eMMC for storage which uses something like 0.5 watts. You can upgrade to NVMe SSD storage but NVMe uses a bit more power. With the low CPU clock speed, I’m curious if NVMe would make much of a difference. My thought is, probably not. Let me know if you benchmark this. **Battery life is great, I’m getting about 8 to 10 hours 6 to 8 hours.**
> 
> @hydnj [https://haydenjames.io/pinebook-pro-my-first-impressions-and-setup-tips/](https://haydenjames.io/pinebook-pro-my-first-impressions-and-setup-tips/)

<script note="" src="https://cdn.jsdelivr.net/gh/Blogger-Peer-Review/quotebacks@1/quoteback.js"></script>

# First small tweaks

The Manjaro team have a few good-to-know things directed at Pinebook Pro owners listed [here](https://forum.manjaro.org/t/tips-tricks-for-your-new-pinebook-pro/145077).

I read [this lovely review-and-tips blog post](https://haydenjames.io/pinebook-pro-my-first-impressions-and-setup-tips/) (even though the poster is on Debian and not Manjaro) and did this:

- [Changed to a new desktop background](https://www.reddit.com/r/wallpapers/comments/bh8loi/pine_38402400/)
- [Changed the default icons](https://snwh.org/paper)

# Installing software

Manjaro Linux is based on Arch Linux. It's not unfair to say Arch has been a distribution for people who know their way around a [Linux shell](https://en.wikipedia.org/wiki/Unix_shell) and know their way around Linux. Manjaro is different.

One of the main things about Manjaro is that it supports a lot of hardware out-of-the-box. I didn't have to search for, install, or configure drivers for a wireless mouse; I just jacked a receiver into a USB port and it worked. The same for connecting my headphones via Bluetooth. No issues.

One thing that I recommend is to [enable the Arch User Repository (AUR)](https://itsfoss.com/aur-arch-linux/) in Manjaro. It's simple and gives you access to a lot of software apart from the regular and official Arch repositories.

Other ways to install software in Manjaro on ARM include Snap and Flatpak, the former of which is [controversial](https://lwn.net/SubscriberLink/825005/6440c82feb745bbe/), to say the least; it also allows installations to balloon far beyond their initial size.

## Running other operating systems from an SD card

Pinebook Pro supports this from the start: I didn't have to configure anything to enable this functionality.

When ordering the laptop I also ordered a 64 GB SD memory. It set me back 20 USD. The laptop allows for running different ARM-compatible operating systems from the SD card, straight off the bat. That's extremely nice and good-to-have! You can download and install any ARM-compatible operating system you want, but I've gone for some Pinebook Pro-compatible ones as I'm really not a Linux tinkerer; PINE64 maintain a radiant list of operating systems [here](https://wiki.pine64.org/index.php/Pinebook_Pro_Software_Release).

To flash an image, I use [balenaEtcher](https://www.balena.io/etcher/), free software that just works. The graphical user interface is simple and very easy to use.

I didn't even have to download an image to flash to the SD card, but I merely entered out the URL to the image; balenaEtcher took care of that in no time. When it was done, I just popped the SD card into the reader in the laptop, hit the power button, and the operating system started up nicely. You can even install Chrome, the operating system that Google use for their Chromebooks.

**Edit, 2020-07-21**: I've noted a tendency where Pinebook Pro boots to the SD card about 30% of the time and [written about it in the Pine64 forum](https://forum.pine64.org/showthread.php?tid=10750).

## Sync

I love sync software. I mean, software that allows you to replicate stuff between different machines, preferably regardless of operating system.

My favourite sync software has since long been **Resilio Sync**. I've paid for a license, and I use it all the time between macOS and Android machines, from laptop to stationary, mobile, and tablet.

My love for Resilio will endure, but it's been dragged through the mud because of how they handle Linux. Let me explain:

I installed Resilio Sync as it was available via AUR. Hell yes! That's where my problems started. [Resilio's Linux guide](https://help.resilio.com/hc/en-us/articles/204762449-Guide-to-Linux) is, to put things mildly, not good. I installed, read that, then reverted to the radiant Manjaro Forums, where I found [this article](https://forum.manjaro.org/t/how-to-install-resilio-sync-aka-rslsync-depreciated-bitorrentsync-bt-sync/22755). Sadly, the article isn't really up-to-speed and having fiddled around with it for a short while, I just decided against Resilio Sync on my Pinebook Pro and went elsewhere.

**[Syncthing](https://syncthing.net/)** saved me.

It's open, cross-platform, encrypted, and there's no man-in-the-middle. [The documentation](https://docs.syncthing.net/users/autostart.html) is well made. I installed `[syncthing](https://www.archlinux.org/packages/community/x86_64/syncthing/)` and `[syncthing-gtk](https://www.archlinux.org/packages/community/any/syncthing-gtk/)`; the former is the binary package and the latter is the graphical user interface.

Arch maintain [this very sweetly written wiki article](https://wiki.archlinux.org/index.php/Syncthing) on Syncthing,

There's [a nice matrix of backup and sync software at Arch Wiki](https://wiki.archlinux.org/index.php/Synchronization_and_backup_programs).

I've not yet managed to configure my system so that it allows the Syncthing updater to start, but I know it's because I've not found out how to add proper rights yet. It'll happen.

## Obsidian (or, rather, not)

I've recently fallen in love with [Obsidian](https://obsidian.md) and have written extensively about it [here](https://niklasblog.com/?p=25043).

Before starting up the Pinebook Pro for the first time, I installed [VirtualBox](https://www.virtualbox.org/) and used it to run Manjaro virtually. I then installed Obsidian without any problems, using the Snap package. Easy, peasy.

It wasn't possible on the Pinebook Pro, I tell you what.

The reason why that is is that I'd not emulated an ARM processor on my VirtualBox. There you go. I've even checked with Obsidian developers. One day they might release an ARM-compatible Obsidian, but not in the near future.

A possible workaround would be to install [Wine](https://www.winehq.org/) and see if it's possible to emulate Obsidian running under Windows; Obsidian is not listed in [their database](https://appdb.winehq.org/), but the day may just come...

Having said this, [Zettlr](https://zettlr.com) is [available for Arch](https://aur.archlinux.org/packages/zettlr-bin/), but not for the aarch64 architecture. In other words: no Zettlr for Pinebook Pro.

Having said that, I went for a workaround:

1. Install Syncthing and have your Obsidian vaults sync around to everywhere you want to access your stuff.
2. Install a Markdown editor to edit your stuff (and see the section below for details on these software)
    - Linux: [Remarkable](https://remarkableapp.github.io/linux.html) or [Kate](https://kate-editor.org/)
    - Android: [Markor](https://play.google.com/store/apps/details?id=net.gsantner.markor&hl=en_US) (as I'm unable to save files using [iA Writer](https://play.google.com/store/apps/details?id=net.ia.iawriter&hl=en))

## Markdown editor

I've recently—since Obsidian, actually—really discovered the many boons of writing in Markdown.

So, one boon of using Syncthing and not being able to use Obsidian, is that I can use a Markdown editor to write, as that's most of what I do.

Naturally, there are [quite a few Markdown editors](https://itsfoss.com/best-markdown-editors-linux/) to choose from. Unfortunately, Typora is not made for the ARM architecture; still, it's not obligatory nor unique, and will cost money after it exits its beta phase.

Having said that, I'm very happy with what I've found.

### Ghostwriter

![](https://niklasblog.com/wp-content/dark-theme.png)

Ghostwriter with dark theme.

**Edit, 2020-07-21**: I wish I'd found [Ghostwriter](https://wereturtle.github.io/ghostwriter/) first.

It's a simple little application that allows you to write in a distraction-free environment. Everything I need, including customisable theming.

It's also got **Hemingway mode** that can be enabled, which only lets you write and not edit; In other words, when enabled, you can't delete or change anything you've written.

Ghostwriter is available via the official Arch repository.

### Remarkable

![](https://remarkableapp.github.io/images/main_screenshot.png)

Remarkable in Gnome.

As stated previously, Remarkable does a great job with displaying vertically-split windows so that you can see what you're editing on one side and a preview of Markdown on the other. Supports themes and 'night mode'.

### Kate

![](https://kate-editor.org/images/xkate-window.png.pagespeed.ic.eOAUieIU_Q.webp)

[Kate](https://kate-editor.org/) is part of KDE, and hence pre-installed with Pinebook Pro and Manjaro.

This is a multi-document editor and is highly customisable.

> With a multi-view editor like Kate you get a lot of advantages. You can view several instances of the same document and all instances are synchronized. Or you can view more files at the same time for easy reference or simultaneous editing.

There are [a lot of features in Kate](https://kate-editor.org/about-kate/), among them, plugins, syntax highlighting, scripting support, and an embedded Terminal.

## Viewing: Okular or Evince

For viewing files, there are a couple of nice apps that I've stumbled across. Let's say that I've not looked around for great apps to view and annotate documents so far, but considering what's available on Windows, these two are brilliant.

![](https://okular.kde.org/images/screenies/okular-backend-pdf-1.png)

Okular on Gnome

[Okular](https://okular.kde.org/) is included with KDE.

It's cross-platform and handles [a lot of different formats](https://okular.kde.org/formats.php).

I like opening Markdown files in this app and having them exported to HTML, PDF, or OpenDocument text (which one can open in Microsoft Word, among many other word processors).

![](https://wiki.gnome.org/Apps/Evince?action=AttachFile&do=get&target=evince-2.png)

Evince

[Evince](https://wiki.gnome.org/Apps/Evince) is a bit more slick than Okular and also [supports quite a few formats](https://wiki.gnome.org/Apps/Evince/SupportedDocumentFormats).

## Shell

![create multiple terminals in terminator window](https://i0.wp.com/www.linuxandubuntu.com/wp-content/uploads/2019/06/create-multiple-terminals-in-terminator-window.jpg?w=1400)

Terminator

I've installed [**Terminator**](http://www.linuxandubuntu.com/home/terminator-a-linux-terminal-emulator-with-multiple-terminals-in-one-window) and not looked back. It's part of the official Arch repository. It allows you to right-select a shell and select 'split horizontal' or 'split vertical', and you can have as many shells running as you want.

## Process viewer

![](https://hisham.hm/htop/htop-2.0.png)

htop

In Windows, this is named Task Manager. In macOS, it's Activity Monitor.

I've installed [**htop**](https://hisham.hm/htop/), an interactive process viewer that's highly customisable. It allows you to select headings to sort the results differently.

htop is available in the official Arch repository.

[This post](https://askubuntu.com/a/312543) conveys some brilliant tips on what to hide from htop.

## Other network-monitoring apps

I'm just going to quote the following from [this brilliant post](https://louisabraham.github.io/articles/pinebook-pro-setup.html):

> I found those two tools very useful:
> 
> - bmon monitors the bandwidth over time
> - nethogs tracks the network usage of every program
> 
> You can install them with pacman.
> 
> [https://louisabraham.github.io/articles/pinebook-pro-setup.html](https://louisabraham.github.io/articles/pinebook-pro-setup.html)

<script note="" src="https://cdn.jsdelivr.net/gh/Blogger-Peer-Review/quotebacks@1/quoteback.js"></script>

## KDE Connect

When I first posted this review I forgot something: [KDE Connect](https://kdeconnect.kde.org/)! How could I when I'm in love with it?

<iframe sandbox="allow-same-origin allow-scripts" src="https://peertube.mastodon.host/videos/embed/f8ffd8de-3df5-46b5-bbe3-114393be4b44" allowfullscreen width="560" height="315" frameborder="0"></iframe>

I mainly use KDE Connect to respond to events in my mobile phone.

You can enable bidirectional copy/paste to have what you copy on your computer delivered to your phone. Transfer files. Check where your phone is. See its battery level. Respond to text messages. Download podcast episodes to your phone. Use KDE Connect as a remote control for your

It's extensible as hell. You can even enter commands to your computer (e.g. power it off) and control slideshows.

## Netflix

You won't be able to watch stuff from Netflix or Amazon without this (unless you apply another custom solution).

[This PINE64-forum post](https://forum.pine64.org/showthread.php?tid=9680&pid=65008#pid65008) solved everything for me.

One has to install Docker and then Chromium with Widevine installed. Then, run Chromium, add the custom Netflix extension, and configure it to always display video in the highest-available format (and to use 5.1 sound if you want to and can).

I've only tried Netflix on it, but it runs like a charm.

## Using video via USB-C

I was keen to try this out and really wondered whether it'd work! I plugged in a third-party USB-C cable that I use for my MacBook Pro, inserted the USB-C end into the Pinebook Pro...and nothing. I pulled up the Display settings in Manjaro, and no additional display was detected.

Hang on.

I unplugged the USB-C cable from the laptop, turned it upside-down, and inserted it.

Presto.

A pristine extended image was displayed on my TV and Manjaro told me I had another display available.

Manjaro surprised me by offering so many display settings. Lovely.

Now, this could be me, but I don't think one is able to send audio via USB-C on the Pinebook Pro. I'd have loved that, but still, I'm happy with what I get. There's an audio port on the Pinebook Pro so I'll use that.

# Performance tricks

## Swapping

Before receiving my Pinebook Pro, I'd checked out [videos](https://www.youtube.com/watch?v=A0WoBMKjc5c) and [blog posts](https://haydenjames.io/pinebook-pro-my-first-impressions-and-setup-tips/) on how to enable [memory swapping](https://en.wikipedia.org/wiki/Paging), which is something that you should do with machines that don't have much memory. The Pinebook Pro has 4 GB of RAM, which isn't a lot. I've owned mobile phones that have had double that size.

Having said that, a lot of operating systems require a lot of RAM. Windows, macOS, what-have-you, they eat through memory.

The aforementioned video mentioned this as a way to check whether swap is configured:

```
cat /proc/meminfo | grep Swap.
```

What do you know, `SwapTotal` was already configured.

## Processor tweaking

![](https://niklasblog.com/wp-content/image-45.png)

Imagine having access to an app that you use to tell your computer's processors to behave differently. Well, now you can.

`cpupower` is available in the official Arch repository and `cpupower-gui` is available in AUR.

Install them both and use the app to switch between different modes to save battery or go full-speed. Using the 'Performance' mode is good for watching Netflix or playing games. 'Conservative' and 'Powersave' are brilliant for just writing.

# Issues

## Keyboard settings

First, I'm Swedish and a Linux noob, which means I wanted to change the keyboard layout. I wanted the system UI to be in British English and the keyboard to be in Swedish.

By the way, this issue has to do with Manjaro and not with PINE64 unless I'm gravely mistaken about how the world works.

I configured **Keyboard settings** to use a _Generic 86-key PC_ Keyboard Model, _Swedish_ as language, and _Swedish (no dead keys)_ as the format.

Said and done. Apply. OK.

Suddenly, while typing away somewhere, it switched.

I suddenly had British English as my keyboard layout again.

I checked **Keyboard settings** again, and, yes, it said I was using British English. I changed it back to Swedish.

Following a reboot I saw British English again.

I actually can't remember how this was resolved in the end, but I resorted to some hacking as via [this page](https://forum.manjaro.org/t/solved-cant-change-locale-after-installation/21675) and also via some user interface. Fingers crossed that this doesn't recur.

## High-pitched (yet quiet) noise from the laptop

There's some sort of high-pitched intermittent squealy noise coming from the computer, and I think it could be related to my wireless mouse.

When the wireless-mouse USB plug is connected to either of the two USB ports of the Pinebook Pro, it squeals.

1. If I disconnect the power cable, the pitch lowers
2. If I then disconnect the USB-plug for my wireless mouse, the pitch lowers even more
3. If I connect a USB cable to any of the ports, there's no noise
4. If I've not had the USB plug connected to any ports for a while, the noise goes away

## Trackpad

The trackpad may not be the best that I've used, but with a good wireless mouse, you'll get everywhere. About eight months ago, ayufan developed [this firmware patch](https://github.com/ayufan-rock64/pinebook-pro-keyboard-updater) to resolve issues that people experienced. I can only say that I think they've since been resolved.

Don't do as I and quickly enter Manjaro Trackpad settings, raise the sensitivity a lot, and apply; This will make the pointer ultra-sensitive, and the risk is that you won't be able to turn it back. I had to plug in a wireless mouse to be able to lower the trackpad sensitivity again, and I'd have cried if I didn't have access to a mouse at the time.

# Summary

Pinebook Pro is a wonderful piece of hardware that is beautifully and thoughtfully crafted. Just check out how sleek it is from above:

![](https://cdn.arstechnica.net/wp-content/uploads/2020/06/IMG_20200602_165330-800x600.jpg)

From [this review in Ars Technica](https://arstechnica.com/gadgets/2020/06/pinebook-pro-review-a-200-foss-to-the-hilt-magnesium-chassis-laptop/). The silvery computer is a Dell XPS 13 DE and Pinebook Pro is to the right (switchblade not included).

200 USD is a lot of money to a lot of people, but it's not much in comparison with a lot of other laptops. The screen size is lovely, the software is wonderful, and the communities of people who are willing to help each other out are vast.

I recommend Pinebook Pro, PINE64, and Linux to anybody who wants freedom in their computing life.
