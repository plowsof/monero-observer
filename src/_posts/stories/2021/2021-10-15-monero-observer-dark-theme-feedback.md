---
layout: post
category: story
title: Looking for new Monero Observer dark theme feedback
description: The Monero Observer will now display a different theme (light or dark) depending on your device or browser settings. 
tags: [meta]
image: mo-dark.png
---

The Monero Observer will now display a different theme (light or dark) depending on your device or browser settings. 

After getting a lot of feedback requesting a dark(er) theme, I was presented with a couple of choices:

1. add (manually) switchable dark theme *(no, requires JS)*
2. stick with original light theme *(no alternative though)*
3. switch to dark theme only *(there are still benefits to light theme)*
4. **add auto switchable light/dark theme** *(no real cons?)*

**Obviously, I went with number 4.**

The reasons I still plan on supporting the original light theme:

- an effort to **not** contribute to Monero's stigma of being a *bad* crypto (used on DNMs and mainly by *criminals*) 
- Getmonero.org official website has a default light theme and I like the legitimate feel it gives

Adding a fully switchable light/dark theme is not an option as I want to keep the website 100% JS-free. 

The best thing I could find was the `prefers-color-scheme` CSS media feature. Most (major) browsers should support this. 

Test it:

- access monero.observer in a browser/device/OS that has *Dark mode* enabled > the site should display the dark theme

- if you access the site using a browser/device with a light theme/mode, it will default to the original light theme

You should be able to set most operating systems, devices and browsers to *Dark mode*.


What do you think? 

As always, any feedback is appreciated.

**-3RA**

---

[^1]: [/changelog](/changelog)
