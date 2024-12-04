---
title : "Windows Update + WSUS"
author : "Niklas"
date : "2005-08-05"
categories : 
 - tech
---

On 2005-08-09 [these patches](http://www.eweek.com/article2/0,1895,1843878,00.asp) will roll out, and six of them are critical. Nothing special about them, actually, but I thought I'd share a little info on [WSUS](http://www.microsoft.com/windowsserversystem/updateservices/default.mspx), the free server application Microsoft made available appx. a month ago, which enables people to carry their own Windows Update-server in their network.

So what makes that better than letting all the clients use Windows Update? Quite a few things:

1\. Administrators approve and deny exactly which updates are sent to the clients. 2. Bandwidth is preserved, as the clients won't download the needed software through Internet. 3. Reporting: administrators see which computers need updates, which ones are protected and can find computers that have failed in applying updates.

I say those are the top three reasons to run a WSUS server. On the other hand, what really makes this work is not a technical issue, but an organisational one. In my work-place we're five network administrators. When a new WU-patch (or update of an old patch) has been released, I immediately ask the other admins if they think we should approve of, or deny this patch. We're all required to answer within a day, and hence the updates are always distributed to the client computers within a day, which is quick.

So why not just let the WSUS-server approve of every update automatically and send what's needed to the client computers? The answer is simple: some of the updates wouldn't help us at every specific time, but create problems instead. We didn't release WinXP SP2 at once, just because that update is so major, that it needed to be thought-through, tested and studied before we applied it. During testing, I found that three of our applications didn't work on WinXP SP2; I contacted the suppliers who made the programs, who all were working on patches of their own, enabling their software to work on SP2. There you go, just a little example. Historically, Microsoft have been quite bad at releasing patches that haven't caused havoc. One had to reinstall computers entirely, and there was no central management of patches until the previous version of WSUS, called SUS. Actually, while beta-testing WSUS it was called WUS. I rue the day they changed the acronym.

It's a good thing, WSUS. Check it out if you're an admin. If you're a home user reading this, you're either too interested in tech or just mad enough to have a few hundred client computers in your home network.
