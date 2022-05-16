---
layout: post
category: story
title: COMIT releases XMR-BTC atomic swap tool v0.10.1
description: COMIT has released version 0.10.1 of their XMR-BTC atomic swap tool.
tags: services
image: 
---

COMIT[^1] has released version 0.10.1[^2] of their XMR-BTC atomic swap implementation[^3].

This update adds a `monero-recovery` command that prints the Monero address, private spend and view key.

It can be used to manually recover instances where the *monero-wallet-rpc* does not pick up the Monero funds locked up by the Automated Swap Backend: 

> The command takes the swap-id as parameter.

> The swap has to be in a BtcRedeemed state.

> Use --help for more details.

Visit Github[^3] to learn more about the tools and join COMIT's Matrix channel[^4] if you need help.

---

[^1]: https://comit.network
[^2]: [https://github.com/comit-network/xmr-btc-swap/releases/tag/0.10.1](https://github.com/comit-network/xmr-btc-swap/releases/tag/0.10.1){:target="_blank"}{:rel="nofollow"}
[^3]: https://github.com/comit-network/xmr-btc-swap
[^4]: https://matrix.to/#/#comit-monero:matrix.org
