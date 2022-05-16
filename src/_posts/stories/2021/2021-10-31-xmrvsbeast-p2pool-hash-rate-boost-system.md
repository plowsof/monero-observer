---
layout: post
category: story
title: xmrvsbeast announces HR boost system for low hash P2Pool miners 
description: xmrvsbeast has announced a hash rate boost system that aims to help low hash P2Pool miners.
tags: mining
image: 
---

xmrvsbeast[^1] has announced[^2] a hash rate boost system[^3] that aims to help low hash P2Pool miners:

> You register your wallet addess and p2pool node, the system works down the list of registered miners and gives a boost to each if conditions are met.

> Make sure to open the stratum port (3333) to your p2pool node in your router and firewall so the remote miners can send you the HR!

Rules:

- your node must have found its last p2pool share in 24-96hrs time window
- you are skipped if you win and your node is down or your have no shares in the time window
- if a share is found before the boost round ends, a new winner is selected

More details about the current boost hash rate, remaining round time and recent boosts can be found on the website[^3].

To get started with P2Pool[^4], consult the Github repository[^5].

---

[^1]: https://libredd.it/r/xmrvsbeast
[^2]: [https://libredd.it/r/moneromining/comments/qjmcwh/](https://libredd.it/r/moneromining/comments/qjmcwh/){:target="_blank"}{:rel="nofollow"}
[^3]: [https://xmrvsbeast.com/p2pool](https://xmrvsbeast.com/p2pool){:target="_blank"}
[^4]: https://p2pool.io/
[^5]: https://github.com/SChernykh/p2pool#how-to-mine-p2pool
