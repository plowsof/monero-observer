---
layout: post
category: story
title: COMIT releases XMR-BTC atomic swap tool v0.10.2
description: COMIT has released version 0.10.2 of their XMR-BTC atomic swap tool.
tags: services
image: 
date: 2021-12-26 20:00
---

COMIT[^1] has released version 0.10.2[^2] of their XMR-BTC atomic swap implementation[^3].

## Changes

- record monero wallet restore blockheight in state SwapSetupCompleted already.
- logs to use rfc3339 local time formatting.

This fixes the underlying issue that was throwing a `No unlocked balance in the specified account` error:

> This solves issues where the CLI went offline after sending the BTC transaction, and the monero wallet restore blockheight being recorded after Alice locked the Monero, resulting in the generated XMR redeem wallet not detecting the transaction [..]

Note that this is a breaking database change and you should finish any priorly saved swaps before upgrading, as they may fail if they are in state `SwapSetupCompleted` of `BtcLocked`.

Visit Github[^3] to learn more about the tools and join COMIT's Matrix channel[^4] if you need help.

---

[^1]: https://comit.network
[^2]: [https://github.com/comit-network/xmr-btc-swap/releases/tag/0.10.2](https://github.com/comit-network/xmr-btc-swap/releases/tag/0.10.2){:target="_blank"}{:rel="nofollow"}
[^3]: https://github.com/comit-network/xmr-btc-swap
[^4]: https://matrix.to/#/#comit-monero:matrix.org
