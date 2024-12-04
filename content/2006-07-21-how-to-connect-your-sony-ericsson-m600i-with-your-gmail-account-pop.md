---
title : "How to connect your Sony Ericsson M600i with your GMail account (POP)"
author : "Niklas"
date : "2006-07-21"
categories : 
 - materialism
 - tech
 - windows
---

This isn't as hard as it seems, if you follow this step-by-step.

1\. [Upgrade the firmware](http://www.sonyericsson.com/support) in your [M600i](http://www.amazon.com/exec/obidos/ASIN/B000GGO5KO/niklasblog-20) if you can't get your machine going by following the steps after this one; my upgrade solved my problems, as it added functions required.

**note**: upgrading your firmware erases everything in your phone. Backup beforehand.

2\. I used [these settings](http://mail.google.com/support/bin/answer.py?answer=13287) to figure out what was up. To simplify things, you need to create a new e-mail account through the messaging-part of your [M600i](http://www.amazon.com/exec/obidos/ASIN/B000GGO5KO/niklasblog-20). After that, you configure the three following parts:

**Basic** `account name: [a name you decide] your name: [your actual name, e.g. Niklas Pivic] email address: [e@mail.nu] connection type: POP3`

**Inbox** `incoming server address: pop.gmail.com username: user@gmail.com password: [yourpassword] download restrictions: no restrictions`

Do note the importance of no restrictions: I remember having read a Google article saying GMail cannot handle requests from e-mail clients asking to merely download the "header" of an e-mail, so there you go.

**Outbox** `outgoing server address: smtp.gmail.com check "Use SMTP authentication" check "Use Inbox login details"`

3\. Now, you're almost done. Click "More" on the lower, right-hand side of the screen and pick "Advanced".

Here, you see two tabs:

**Incoming** `secure connection: SSL incoming mail port: 995 leave "Secure password authentication" unchecked`

**Outgoing** `secure connection: TLS outgoing mail port: 587 check the box marked "use MIME encoding" (I did, anyway)`

That should do it, go!
