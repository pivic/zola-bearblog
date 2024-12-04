---
title : "Amazon Kindle Oasis 2: “UPDATE ERROR 4” after a manual firmware update attempt"
author : "Niklas"
date : "2019-07-10"
categories : 
 - health
 - materialism
 - tech
---

![](https://niklasblog.com/wp-content/all-new-kindle-oasis-the-goods.jpg)

I recently updated my Amazon Kindle with the latest firmware.

When doing so, I used a different cable than the one that Amazon provided me with. I am now quite sure that the cable I used for the operation was subpar; this probably resulted in corruption of the .bin file—i.e. the Kindle firmware update file—that _appeared_ to have been successfully transferred to the device.

Thus, my nightmare began. This post is an attempt to warn people of what can happen when failing to manually update the Kindle.

First, the non-manual method is to enable Wi-Fi and have the device download and update itself. If you're like me, a techie who enjoys performing manual updates as the over-the-air (OTA) method is both slower and not available as soon as the .bin file is made available to manually download, this is not a boon.

If you manually download the .bin file, there are two things that can go wrong with it:

1. it can corrupt during transfer from Amazon's servers to where you save it
2. it can corrupt during transfer from your saved location to the Kindle

Currently, Amazon save their .bin files [here](https://www.amazon.com/gp/help/customer/display.html?nodeId=200529680), and I believe they once provided MD5 checksums for those files but I can't find them now. For non-techies, MD5 checksum is the following, [via Wikipedia](https://en.wikipedia.org/wiki/MD5):

MD5 digests have been widely used in the [software](https://en.wikipedia.org/wiki/Software) world to provide some assurance that a transferred file has arrived intact. For example, file servers often provide a pre-computed MD5 (known as [md5sum](https://en.wikipedia.org/wiki/Md5sum)) [checksum](https://en.wikipedia.org/wiki/Checksum) for the files, so that a user can compare the checksum of the downloaded file to it. Most unix-based operating systems include MD5 sum utilities in their distribution packages; Windows users may use the included [PowerShell](https://en.wikipedia.org/wiki/PowerShell) function "Get-FileHash", install a Microsoft utility, or use third-party applications. Android ROMs also use this type of checksum.

In my case, I didn't verify the checksum, which means I had no chance to know whether the .bin file was OK or corrupt.

Upon updating my fully-charged Kindle, the following happened:

1. it restarted
2. it started the firmware update process as usual
3. it displayed the person-reading-under-a-tree picture with no progress bar, with the backlight on maximum

![](https://niklasblog.com/wp-content/Screenshot-2019-07-10-at-13.48.05.png)

Like this, but the backlight glaring like the sun.

[I tried pressing the power button for a minute](https://www.amazon.com/gp/help/customer/display.html/?nodeId=200829000) and then let go; that didn't result in anything but the screen flickering once, then reverting to what happened in step three above.

I tried pressing the power button for four minutes, then let go; the result was the same as with pressing it for a minute.

[A support article on Amazon's site](https://www.amazon.com/gp/help/customer/display.html/?nodeId=200829000) suggested to charge the Kindle for at least 30 minutes and then retry to restart it. I did, and I did, with the same results as above.

Connecting the Kindle to a computer by use of an Amazon-provided USB cable didn't result in anything; this was one of the first questions that Amazon's American support team asked me, by the way. They didn't ask any follow-up questions but assessed that my Kindle was now [bricked](https://en.wikipedia.org/wiki/Brick_(electronics)), which I think was correct of them.

Another thing: contact Amazon depending on which country you have bought your Kindle from.

I bought mine from Italy and was asked to contact them. They don't offer chat as a support method, but quickly answered my e-mail in the morning and plainly asked me to call them for support.

However, here's the best part about all of this:

When I, irritated and grumpy, went to bed and had simply placed my Kindle somewhere with its lid closed —which under regular circumstances enables sleep mode, but actually hadn't as the firmware-update error prevented it from going to sleep—I thought I'd have to wait for ages until receiving a new Kindle, etc.

I woke up and checked my Kindle. It woke from sleep, as before the problems started.

It just asked me for my PIN code, as it usually does.

GOD EXISTS

OK, hold up. _God is a social construct._

When I'd entered my PIN code, I could see two books. Kindle then threw me a message saying something like it'd "encountered irreparable issues", and yes, I had no books on my device.

I connected the Kindle to my computer, using a USB cable that's OK, and it instantly connected as it usually does.

It told me I had 6.66 GB available free space.

Satan exists.

So, I naturally did what any insane person would, and manually performed a firmware update. I downloaded the .bin file from scratch, didn't check the MD5 checksum, transferred the file to the root directory of my Kindle, tried to update it, and hey, that worked.

After that I had to transfer books back to the Kindle, and...it worked. It's worked since.

In other words:

- don't use a dodgy USB cable to update your firmware manually
- use the OTA method to update the firmware on your Kindle
- verify the MD5 checksum of the downloaded firmware to verify that it's an OK file (and don't ask me how to find the checksum - ask Amazon).

Advice to Amazon:

- allow the Kindle to perform the same MD5 checksum verification that it does when OTA-downloading firmware when manually updating the firmware
- publish the MD5 checksums for all Kindle firmware online
