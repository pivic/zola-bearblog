---
title : "Fawkes: mask your face against facial-recognition software"
author : "Niklas"
date : "2020-07-23"
categories : 
 - health
 - heroes
 - insane
 - people
 - photo
 - politics
 - tech
---

![](https://niklasblog.com/wp-content/image-46.png)

[Fawkes](http://sandlab.cs.uchicago.edu/fawkes/) is a new piece of software that works to mask your facial pictures from being tracked even if they're online.

[This blog post](https://onezero.medium.com/i-got-my-file-from-clearview-ai-and-it-freaked-me-out-33ca28b5d6d4) is written by a man named Thomas Smith. He told clearview.ai to give him his data. First, what do companies like Clearview—notably Amazon, Facebook, Twitter, Google, and Microsoft—snatch and do?

> In a matter of seconds, Clearview locates the person in its database using only their face. It then provides their complete profile back to the client. As of early 2020, the company had more than [2,200 customers using its service](https://www.theverge.com/2020/2/27/21156678/clearview-ai-client-macy-fbi-doj-twitter-facebook-youtube).
> 
> What does a Clearview profile contain? Up until recently, it would have been almost impossible to find out. Companies like Clearview were not required to share their data, and could easily build massive databases of personal information in secret.
> 
> Thanks to two landmark pieces of legislation, though, that is changing. In 2018, the European Union began enforcing the [General Data Protection Regulation](https://gdpr-info.eu/) (GDPR). And on January 1, 2020, an equivalent piece of legislation, the [California Consumer Privacy Act](https://oag.ca.gov/privacy/ccpa) (CCPA), went into effect in my home state.
> 
> Thomas Smith [https://onezero.medium.com/i-got-my-file-from-clearview-ai-and-it-freaked-me-out-33ca28b5d6d4](https://onezero.medium.com/i-got-my-file-from-clearview-ai-and-it-freaked-me-out-33ca28b5d6d4)

<script note="" src="https://cdn.jsdelivr.net/gh/Blogger-Peer-Review/quotebacks@1/quoteback.js"></script>

It's safe to say they had a lot of his pictures, trawled from places like Facebook and Twitter. Clearview scrape pictures from everywhere.

There were a slew of hits:

![](https://miro.medium.com/max/1400/0*yvZfd4G7cTp2N06y)

![](https://miro.medium.com/max/1400/0*DU6A7c_H8ESaU55r)

There's an erroneous hit in there.

Imagine what would be the case if you're a person of colour. Does that matter?

> Researchers say facial recognition software is up to 100 times more likely to misidentify people of color than white people. This week, Boston voted to end its use in the city, and Democratic lawmakers introduced a similar measure for federal law enforcement. “This is not an example of one bad algorithm. Just like instances of police brutality, it is a glimpse of how systemic racism can be embedded into AI systems like those that power facial recognition technologies,” says Joy Buolamwini, founder of the Algorithmic Justice League.
> 
> @democracynow [https://www.democracynow.org/2020/6/26/racist\_facial\_recognition\_technology\_joy\_buolamwini](https://www.democracynow.org/2020/6/26/racist_facial_recognition_technology_joy_buolamwini)

<script note="" src="https://cdn.jsdelivr.net/gh/Blogger-Peer-Review/quotebacks@1/quoteback.js"></script>

It matters extremely much.

This is why a tool like Fawkes is important. What does it do?

> The [SAND Lab](http://sandlab.cs.uchicago.edu/) at University of Chicago has developed _**Fawkes**_, an algorithm and software tool (running locally on your computer) that gives individuals the ability to limit how their own images can be used to track them. At a high level, Fawkes takes your personal images, and makes tiny, pixel-level changes to them that are invisible to the human eye, in a process we call _image cloaking_. You can then use these "cloaked" photos as you normally would, sharing them on social media, sending them to friends, printing them or displaying them on digital devices, the same way you would any other photo. The difference, however, is that if and when someone tries to use these photos to build a facial recognition model, "cloaked" images will teach the model an highly distorted version of what makes you look like you. The cloak effect is not easily detectable, and will not cause errors in model training. However, when someone tries to identify you using an unaltered image of you (e.g. a photo taken in public), and tries to identify you, they will fail.
> 
> Fawkes has been tested extensively and proven effective in a variety of environments, and shows 100% effectiveness against state of the art facial recognition models (Microsoft Azure Face API, Amazon Rekognition, and Face++). We are in the process of adding more material here to explain how and why Fawkes works. For now, please see the link below to our technical paper, which will be presented at the upcoming [USENIX Security Symposium](https://www.usenix.org/conference/usenixsecurity20), to be held on August 12 to 14.
> 
> [http://sandlab.cs.uchicago.edu/fawkes/](http://sandlab.cs.uchicago.edu/fawkes/)

<script note="" src="https://cdn.jsdelivr.net/gh/Blogger-Peer-Review/quotebacks@1/quoteback.js"></script>

As you can see from the image at the top, there's really no difference from the original and the cloaked copy.

Naturally, when a tool like this is openly available, you can bet your life that the companies that are mainly into facial recognition will work to break the code, as it were.

Download links, setup, and use instructions are available [here](http://sandlab.cs.uchicago.edu/fawkes/).

For protesters, it's great to use Fawkes combined with something like [Image Scrubber](https://everestpipkin.github.io/image-scrubber/), which removes EXIF data from images, e.g. GPS-location data and other identification data.
