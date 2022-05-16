---
layout: post
category: story
title: COMIT publishes XMR-BTC atomic swap tool v0.10.0-alpha pre-release
description: COMIT has pre-released version 0.10.0-alpha of their XMR-BTC atomic swap tool.
tags: services
image: 
---

COMIT[^1] has published the 0.10.0-alpha[^2] pre-release of their XMR-BTC atomic swap implementation[^3].

The *Automated Swap Backend* (ASB) will no longer function as a rendezvous server, but it can still register with rendezvous servers as usual.

This update also removes support for the old sled database:

> The ASB and CLI only support the new sqlite database.
> If you haven't already, you can migrate your old data using the 0.9.0 release.

---

[^1]: https://comit.network
[^2]: [https://github.com/comit-network/xmr-btc-swap/releases/tag/0.10.0](https://github.com/comit-network/xmr-btc-swap/releases/tag/0.10.0){:target="_blank"}{:rel="nofollow"}
[^3]: https://github.com/comit-network/xmr-btc-swap
