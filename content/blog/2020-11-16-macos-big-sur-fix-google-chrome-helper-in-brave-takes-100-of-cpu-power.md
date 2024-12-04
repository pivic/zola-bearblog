---
title : "macOS Big Sur fix: Google Chrome Helper (in Brave) takes 100% of CPU power"
author : "Niklas"
date : "2020-11-16"
categories : 
 - tech
---

![drawing](https://niklasblog.com/wp-content/Turn-ideas-into-products.png)

I updated macOS on my laptop to [Big Sur](https://www.apple.com/macos/big-sur/) as soon as I could.

## Problem description

First thing that happened: the laptop fan sped up to the max and the CPU reached 99-100%.

When I used [Activity Monitor](https://support.apple.com/en-gb/guide/activity-monitor/welcome/mac) to check what was going on, I saw a process with the name **Google Chrome Helper** that was eating every bit of CPU that it could.

Bear in mind: I'd updated and upgraded all of my applications and Chromium extensions before upgrading from Catalina to Big Sur.

## Google Chrome Helper

So, what is Google Chrome Helper?

> "Google Chrome Helper" is the generic name for embedded content that runs outside the browser. Browser plug-ins aren't features that are rendered by HTML code; they involve content that needs to be pulled in from elsewhere. The "Google Chrome Helper" is the interface between the embed code in the browser and a remote server, and it's set to run automatically with Chrome's default settings. In many cases, the plug-ins and processes they're handling aren't listed by name because the APIs don't allow it. Google Chrome Helper is a martyr.
> 
> Tim Moynihan [https://www.wired.com/2014/10/google-chrome-helper/](https://www.wired.com/2014/10/google-chrome-helper/)

<script note="" src="https://cdn.jsdelivr.net/gh/Blogger-Peer-Review/quotebacks@1/quoteback.js"></script>

In other words: Google Chrome Helper can run haywire if one or more of your extensions are wonky.

The classic approach: disable all of your extensions and enable them again while keeping an eye on Activity Monitor; a CPU spike in Google Chrome Helper will let you know what's going on.

I use **Brave** to browse and don't even have Chrome installed. [Brave](https://brave.com/) is based on [Chromium](https://www.chromium.org/Home)—an open-source web-browser project—and is a _lot_ more privacy-oriented than Chrome is. Ditch Chrome for Brave if you haven't already; I recommend it.

## My troubleshooting method

1. Update everything in macOS App Store (including Big Sur, even though there aren't any updates available at the time of writing this).
2. Update Brave.
3. Disable all of my extensions.
4. Open Activity Monitor and use force quit to kill the Google Chrome Helper process.
5. Disable one Brave extension.
6. Look at Activity Monitor: does any Google Chrome Helper process pop up again? If no, let the extension be enabled and repeat steps 3-4 with a new extension. If yes, you've most likely found the extension that doesn't seem to work with macOS Big Sur, in some way.

## My result

I didn't have to remove any extensions to get this to work.

The problem hasn't recurred after I disabled all of my extensions and then enabled them.

Weird.

Still, I leave this little tale here so that others may find solace.
