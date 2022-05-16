---
layout: post
category: story
title: COMIT XMR-BTC atomic swap tool version 0.8.3 fixes two significant bugs
description: COMIT has released version 0.8.3 of their XMR-BTC atomic swap tool, which includes two bug fixes.
tags: services
image: 
---

COMIT[^1] has released version 0.8.3[^2] of their XMR-BTC atomic swap tool[^3], which fixes two significant bugs. 

The update mitigates both potential scenarios where:

- the XMR could stay locked up forever while the CLI refunded the BTC

- the CLI is forced to wait for cancel, even though the cancel timelock is not yet expired and the swap could still be redeemed

---

[^1]: https://comit.network
[^2]: [https://github.com/comit-network/xmr-btc-swap/releases/tag/0.8.3](https://github.com/comit-network/xmr-btc-swap/releases/tag/0.8.3){:target="_blank"}{:rel="nofollow"}
[^3]: https://github.com/comit-network/xmr-btc-swap
