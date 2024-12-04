---
title : "Zoom: avoid being tracked in detail"
author : "Niklas"
date : "2020-03-23"
categories : 
 - culture
 - links
 - tech
 - video
---

![](https://niklasblog.com/wp-content/image-19.png)

2020b. “Video Conferencing, Web Conferencing, Webinars, Screen Sharing.” Zoom Video. March 23, 2020. https://zoom.us/.

Zoom has become one of the most—if not _the_ most—popular video-conferencing tools in modern time.

Install one of their apps—for desktop or mobile—and you can easily join a meeting.

Is there any catch to all of this?

* * *

Zoom do not only provide a video-conferencing tool for their customers but also analytics and statistics. It also sells your personal experience; [from Proton Technologies:](https://protonmail.com/blog/zoom-privacy-issues/)

> In its [privacy policy](https://zoom.us/privacy), under the entry “Does Zoom sell Personal Data?” the policy says, “Depends what you mean by ‘sell.’” To summarize Zoom’s policy, they say they don’t sell personal data for money to third parties, but **it does share personal data with third parties for those companies’ “business purposes.”** And that may include passing your personal information to Google. 
> 
> Koch, Richie. 2020. “Zoom Video Conferences Aren’t As Private As You Think.” ProtonMail Blog. March 20, 2020. [https://protonmail.com/blog/zoom-privacy-issues/](https://protonmail.com/blog/zoom-privacy-issues/).

From EFF:

> The host of a Zoom call has the capacity to[ monitor the activities of attendees](https://support.zoom.us/hc/en-us/articles/115000538083-Attendee-attention-tracking) while screen-sharing. This functionality is available in Zoom version 4.0 and higher. If attendees of a meeting do not have the Zoom video window in focus during a call where the host is screen-sharing, after 30 seconds the host can see indicators next to each participant’s name indicating that the Zoom window is not active.
> 
> Oliver, Lindsay. 2020. “What You Should Know About Online Tools During The COVID-19 Crisis.” Electronic Frontier Foundation. March 19, 2020. [https://www.eff.org/deeplinks/2020/03/what-you-should-know-about-online-tools-during-covid-19-crisis](https://www.eff.org/deeplinks/2020/03/what-you-should-know-about-online-tools-during-covid-19-crisis).

I understand why companies would want to know why a certain percentage of attendees doze off mid-presentation. The company could then hone their future presentations to make sure that people stay engaged.

On the other side, this is disconcerting:

> For any meeting that has occurred or is in-process, Zoom allows administrators to see the operating system, IP address, location data, and device information of each participant. This device information includes the type of machine (PC/Mac/Linux/mobile/etc), specs on the make/model of your peripheral audiovisual devices like cameras or speakers, and names for those devices (for example, the user-configurable names given to AirPods). Administrators also have the ability to join any call at any time on their organization’s instance of Zoom, without in-the-moment consent or warning for the attendees of the call.
> 
> Oliver, Lindsay. 2020. “What You Should Know About Online Tools During The COVID-19 Crisis.” Electronic Frontier Foundation. March 19, 2020. [https://www.eff.org/deeplinks/2020/03/what-you-should-know-about-online-tools-during-covid-19-crisis](https://www.eff.org/deeplinks/2020/03/what-you-should-know-about-online-tools-during-covid-19-crisis).

In other words, Zoom will register a lot of your information if you use their apps. Use their web client, and you won't be tracked as much.

* * *

I recently found Arkadiy Tetelman's [Zoom redirector](https://github.com/arkadiyt/zoom-redirector), a small browser extension that redirects Zoom meeting links to use the web client instead of the desktop/mobile app.

It's currently available for Chrome and Firefox, and Arkadiy has submitted it for Opera and Edge.

There are other technologies for meeting via videoconference, for example:

- [Jitsi Meet](https://meet.jit.si/)
- [openVidu](https://openvidu.io/)
- [around](https://www.around.co/)

* * *

Bonus round: for those of you who enjoy security, be aware that Zoom was not only plagued by a sickening security vulnerability less than a year ago, but that they included a web server in their product to bypass Apple Safari security features:

> Last year, security consultant [Johnathan Leitschuch](https://medium.com/bugbountywriteup/zoom-zero-day-4-million-webcams-maybe-an-rce-just-get-them-to-visit-your-website-ac75c83f4ef5) discovered that Zoom set up a local web server on a user’s Mac device that allowed Zoom to bypass security features in Safari 12. This web server was not mentioned in any of Zoom’s official documentation. It was used to bypass a pop-up window that Safari 12 would show before it turned on your device’s camera.
> 
> However, this remote web server was also not adequately secured. Pretty much any website could interact with it. The result was that Zoom allowed malicious websites to take over your Mac’s camera without ever alerting you.
> 
> Koch, Richie. 2020. “Zoom Video Conferences Aren’t As Private As You Think.” ProtonMail Blog. March 20, 2020. [https://protonmail.com/blog/zoom-privacy-issues/](https://protonmail.com/blog/zoom-privacy-issues/).

https://twitter.com/mathowie/status/1148391109824921600

https://twitter.com/xnyhps/status/1149630190877696001

> As Zoom becomes the standard video conferencing tool, there are some steps you can take to keep your data safe.
> 
> **Use two devices during Zoom calls:** If you are attending a Zoom call on your computer, use your phone to check your email or chat with other call attendees. This way you will not trigger the attention tracking alert.
> 
> **Do not use Facebook to sign in: **It might save time, but it is a poor security practice and dramatically increases the amount of personal data Zoom has access to. 
> 
> **Keep your Zoom app updated: **Zoom removed the remote web server from the latest versions of its apps. If you recently downloaded Zoom, there’s no need to be concerned about this specific vulnerability.
> 
> Koch, Richie. 2020. “Zoom Video Conferences Aren’t As Private As You Think.” ProtonMail Blog. March 20, 2020. [https://protonmail.com/blog/zoom-privacy-issues/](https://protonmail.com/blog/zoom-privacy-issues/).
