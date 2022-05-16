---
layout: post
category: story
title: "RogueMaven shares spec for Tails-like 'Monero Ilaro' Linux OS"
description: "RogueMaven has shared the spec document for Tails-like Monero Ilaro Linux OS."
tags: mining
image: monero-ilaro-cli.png
---

RogueMaven[^1] has shared[^2] the spec document for Tails[^3]-like *Monero Ilaro*[^4] Linux OS:

> The ability to plug a USB stick into any computer and temporarily turn it into an XMR miner, p2pool node, and/or monero blockchain node. A simple reboot and the computer is returned back to normal. Essential applications for using Monero will be included in this toolkit (Ilaro).

According to the dev, Monero Ilaro is *ready now*:

> I’m currently using it in my own rig setup.

> All features described in the GitHub spec document are functional and have been tested on many different types of computers. 

Here are my notes for this project (collected from ANN thread[^3] & repo README[^4]):

- Ilaro ISO file can be burned to CD or flashed to a USB stick (~200 MB)
- platform is a customized Alpine Linux distro with APK package system
- installs to RAM (~100 MB at startup)
- Tor support is listed at the top of the to-do list
- can be used offline for benchmark purposes
- BIOS and EFI motherboard bootloader compatible
- will boot on any x86_64 CPU hardware
- persistence is an option
- Docker is required for the build process and to contribute to future development
- update system, documentation, verification, all are WiP/TBD

RogueMaven has expressed some interest in opening up a CCS proposal for this project.

To share your feedback, read the *origin story*, the technical summary and maybe donate some XMR, visit Reddit[^2] and Github[^4]. 



---

[^1]: https://github.com/RogueMaven/
[^2]: https://libredd.it/r/Monero/comments/rdtnii/
[^3]: https://tails.boum.org/install/index.en.html
[^4]: [https://github.com/RogueMaven/monero-ilaro-spec](https://github.com/RogueMaven/monero-ilaro-spec){:target="_blank"}{:rel="nofollow"}
