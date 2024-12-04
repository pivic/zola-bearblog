---
title : "How to migrate from Authy to Aegis"
author : "Niklas"
date : "2021-05-28"
categories : 
 - macosx
 - tech
---

![](https://niklasblog.com/wp-content/2021-05-28_aegis-2048x1252.png)

When I today read [this](https://github.com/pluja/awesome-privacy) lovely privacy-oriented GitHub collection of bad and good apps and services, I came across this:

* * *

## 2FA

[](https://github.com/pluja/awesome-privacy/blob/main/misc/forbidden.png) Avoid using apps that won't let you export your keys **easily**.

- Authy
- Google Authenticator

[](https://github.com/pluja/awesome-privacy/blob/main/misc/check.png) Instead use

- [Aegis](https://getaegis.app/) - A free, secure and open source app for Android to manage your 2-step verification tokens. Supports variety of imports from other apps (Google Authenticator, Authy etc.), vault encryption and exporting keys (plaintext or encrypted).
- [andOTP](https://github.com/andOTP/andOTP) - Open source two-factor authentication for Android.
- [FreeOTPPlus](https://github.com/helloworld1/FreeOTPPlus) - Enhanced fork of FreeOTP-Android providing a feature-rich 2FA authenticator.
- [RavioOTP](https://github.com/raivo-otp/) - A native, lightweight and secure one-time-password (OTP) solution for **iOS** users.

* * *

Hm. I've been using Authy for Android for quite some time, and it contains a lot of my 2FA codes.

Authy syncs across multiple devices, which is nice, but it doesn't allow you to export your 2FA accounts to be used in other apps, which is bad.

There are other bad things about Authy, all listed in [this Hacker News post](https://news.ycombinator.com/item?id=25803996).

So, I thought: why not try Aegis?

## Why Aegis?

There are several good reasons to use [Aegis](https://getaegis.app/):

- It's completely free, both as in free beer and free thought.
- It supports biometric and PIN as security.
- Exports 2FA accounts either as encrypted file or by allowing other apps to scan QR codes.

## How migrate from Authy to Aegis?

This is not entirely simple. Authy don't supply functionality to do this, not via the Android app nor their desktop app.

I use a Mac, and as it happens, a gentleperson has written [this step-by-step guide](https://gist.github.com/gboudreau/94bb0c11a6209c82418d01a59d958c93#gistcomment-3339661) on how to migrate from Authy to [Bitwarden](https://bitwarden.com/), which is a password manager that I highly recommend.

The guide allows you to do two things more than use Bitwarden, specifically:

1. Follow it and it will display QR codes for all of your Authy accounts. Just use the Aegis app to scan them and you're done.
2. You can have Authy save a file that contains a JSON export of all of your 2FA accounts; follow the aforementioned guide, and when you follow step 4 and paste code, exclude the two slash characters in the very last line; when you hit Enter to execute the code, switch to your Authy app: it should display a dialog box that asks you where to save your JSON file.

Aah. The fresh air of freedom.

Thanks to [Guillaume Boudreau](https://gist.github.com/gboudreau) for the original instructions to export Authy data and to [Jesse Calvillo](https://gist.github.com/jcalvillo) for the macOS/Bitwarden tweaks. And, of course, also to [PLUJA](https://github.com/pluja) for their _[Awesome Privacy](https://github.com/pluja/awesome-privacy)_ repo on GitHub.
