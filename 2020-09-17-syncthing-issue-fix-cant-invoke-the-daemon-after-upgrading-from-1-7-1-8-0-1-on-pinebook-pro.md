---
title : "Syncthing issue fix: ‘Can’t invoke the daemon’ after upgrading from 1.7-1.8.0-1 on Pinebook Pro"
author : "Niklas"
date : "2020-09-17"
categories : 
 - linux
 - tech
---

![](https://niklasblog.com/wp-content/2880px-SyncthingLogoHorizontal.svg_-1.png)

**tl;dr**: Linux veterans know how to do these things without flinching; this is a post for neophytes like myself.

A couple of weeks ago I posted the following [in the Syncthing forum](https://forum.syncthing.net/t/cant-invoke-the-daemon-after-upgrading-from-1-7-1-8-0-1/):

* * *

Today I upgraded Syncthing 1.7.x (can’t remember the exact version) on Manjaro (kernel version 5.8.3-2-MANJARO-ARM) running on a Pinebook Pro; I upgraded to Syncthing 1.8.0-1.

When I now start the computer, Syncthing GTK (version 1:0.9.4.4-2) says the following:

Failed to start Syncthing daemon. Error message: Daemon exists too fast

Please, check your installation or set new path to Syncthing daemon binary.

The path that exists - /usr/bin - actually does exist, as does ‘syncthing’ in that location.

I’ve also successfully reinstalled the application, to no avail.

The logs:

panic: qtls.ClientSessionState not compatible with tls.ClientSessionState  
  
goroutine 1 \[running\] [github.com/lucas-clemente/quic-go/internal/handshake.init.2()](http://github.com/lucas-clemente/quic-go/internal/handshake.init.2()) [github.com/lucas-clemente/quic-go@v0.17.3/internal/handshake/unsafe.go:26](http://github.com/lucas-clemente/quic-go@v0.17.3/internal/handshake/unsafe.go:26) +0x1d0

* * *

One of the 'Syncthing Maintainers' said this:

> You have an incorrectly built Syncthing that doesn’t work. Try grabbing one of our binaries from [syncthing.net/downloads](http://syncthing.net/downloads), or downgrade back to 1.7.0, or wait for your distribution to release a fixed package / 1.9.0 release.

My issue: I couldn't sort out how to 'grab a binary' would help me, so here's a step-by-step instruction that resolved my issue (for the Pinebook Pro, mind you; be sure to pick a binary download that suits your processor):

1. Head to [https://syncthing.net/downloads](https://syncthing.net/downloads/)/
2. Select **ARM64**.  
    A .gz file is now downloaded.
3. Decompress the downloaded file.  
    This creates a folder that contains something like the following structure:

![](https://niklasblog.com/wp-content/image-55.png)

4\. Copy or move the file named **syncthing** into /usr/bin/syncthing—or where your syncthing exists—and overwrite the existing one.  
5\. If you run **Syncthing-GTK** (you should if you don't), use it to restart the Syncthing daemon; otherwise, restart your computer, and all should work.

I actually downloaded the latest release-candidate file—currently in [v1.10.0-rc3](https://github.com/syncthing/syncthing/releases/tag/v1.10.0-rc.3)—and it worked perfectly.
