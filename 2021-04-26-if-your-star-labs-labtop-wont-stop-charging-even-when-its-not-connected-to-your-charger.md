---
title : "If your Star Labs LabTop won’t stop ‘charging’ (even when it’s not connected to your charger)"
author : "Niklas"
date : "2021-04-26"
categories : 
 - tech
---

![](https://niklasblog.com/wp-content/IV-UK-04x2000-1.png)

I recently discovered that the red LED on my Star Labs LabTop IV was always on, regardless whether the machine was charging, fully charged, or disconnected from all kinds of cords.

To make matters worse, Manjaro told me the machine was charging when it wasn't connected to any cord.

I contacted Star Labs support who courteously and quickly answered me:

> It sounds like the EC has stalled. To reset it, start with the laptop turned off and then press and hold `Ctrl` + `Alt` + `Del` + `Power` until the LED's on the left side of the laptop flash

This worked. I pressed the key combination, the lights on the left side of the laptop went off and on, I released the keys, and all was well: the red light switched off.
