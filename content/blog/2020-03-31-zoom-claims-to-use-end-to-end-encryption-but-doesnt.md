---
title : "Zoom claims to use end-to-end encryption but doesn’t"
author : "Niklas"
date : "2020-03-31"
categories : 
 - people
 - tech
 - video
---

![](https://niklasblog.com/wp-content/image-19.png)

Can there be one day when Zoom isn't [plagued with lying](https://niklasblog.com/?p=24400), [selling your personal experience to Facebook](https://niklasblog.com/?p=24469), or [installing rogue software on your computer that unleashes a massive privacy bug](https://niklasblog.com/?p=24400)? Please?

Today I learned this, via The Intercept:

> Still, Zoom offers reliability, ease of use, and at least one very important security assurance: As long as you make sure everyone in a Zoom meeting connects using “computer audio” instead of calling in on a phone, the meeting is secured with end-to-end encryption, at least according to Zoom’s [website](https://zoom.us/security), its [security white paper](https://zoom.us/docs/doc/Zoom-Security-White-Paper.pdf), and the user interface within the app. But despite this misleading marketing, the service actually does not support end-to-end encryption for video and audio content, at least as the term is commonly understood. Instead it offers what is usually called transport encryption, explained further below.
> 
> Lee, Micah, and Yael Grauer. 2020. “Zoom Meetings Aren’t End-to-End Encrypted, Despite Misleading Marketing.” The Intercept. March 31, 2020. [https://theintercept.com/2020/03/31/zoom-meeting-encryption](https://theintercept.com/2020/03/31/zoom-meeting-encryption)/.

The Intercept explains further:

> The encryption that Zoom uses to protect meetings is TLS, the same technology that web servers use to secure HTTPS websites. This means that the connection between the Zoom app running on a user’s computer or phone and Zoom’s server is encrypted in the same way the connection between your web browser and this article (on https://theintercept.com) is encrypted. This is known as transport encryption, which is different from end-to-end encryption because the Zoom service itself can access the unencrypted video and audio content of Zoom meetings. So when you have a Zoom meeting, the video and audio content will stay private from anyone spying on your Wi-Fi, but it won’t stay private from the company.
> 
> Lee, Micah, and Yael Grauer. 2020. “Zoom Meetings Aren’t End-to-End Encrypted, Despite Misleading Marketing.” The Intercept. March 31, 2020. [https://theintercept.com/2020/03/31/zoom-meeting-encryption](https://theintercept.com/2020/03/31/zoom-meeting-encryption)/.

I recommend that you read the article by The Intercept where we quickly learn of how Zoom, yet again, try and evade what they mean. Zoom's spokesperson refers to _their own servers_ as 'end points' even though they're not.

When a company makes you feel ill, you know something's up, right?
