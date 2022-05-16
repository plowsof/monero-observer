---
layout: post
category: story
title: PacificNWVet pays 3.93 XMR fee for transferring 0.34 XMR
description: "PacificNWVet has paid an extremely high fee of 3.93 XMR for transferring 0.34 XMR."
tags: events
image: 
last_modified_at: 2022-01-08
---

PacificNWVet[^1] has paid an extremely high fee of 3.93 XMR for transferring 0.34 XMR:

> 3.93 xmr transaction fee for .34 transaction seems way to high and hopefully this is something that does not happen ever to anyone else.. it was 800 dollars approximately transaction fee for a 70 dollar transaction..[^2]

The transaction was sent with the official Monero GUI wallet (Oxygen Orion v0.17.2.0) in *Simple mode* (connected to an unknown remote node) and it was mined by MineXMR[^3].

According to xnbya[^4], the pool's admin, the *block reward has already been distributed to miners*, so a refund is not possible.

It is unclear how this happened, but we need to avoid similar situations from occurring in the future.

selsta[^5] suggested some ideas:

- Warn the user if the fee seems too high.
- Let GUI simple mode only connect to "trusted" remote node.

Also make sure to always verify the fee before sending any transaction, connect to a trusted remote node (or run your own node) and always use the latest wallet version.

If you want to help PacificNWVet, feel free to donate some XMR to his address[^6].

---

**Update: the community has covered the full amount lost in fees[^7].**

---

[^1]: https://github.com/PacificNWVet
[^2]: [https://github.com/monero-project/monero/issues/8134](https://github.com/monero-project/monero/issues/8134){:target="_blank"}{:rel="nofollow"}
[^3]: https://minexmr.com/
[^4]: https://github.com/xnbya
[^5]: https://github.com/selsta
[^6]: https://github.com/monero-project/monero/issues/8134#issuecomment-1007661228
[^7]: https://github.com/monero-project/monero/issues/8134#issuecomment-1007878121
