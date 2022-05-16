---
layout: post
category: story
title: "xmrmfjj2 tricked into paying exorbitant 19.73 XMR transaction fee by malicious remote node" 
description: "xmrmfjj2 was tricked into paying an exorbitant 19.73 XMR transaction fee by a malicious Monero remote node."
tags: events
image: xmrmfjj2.png
date: 2022-04-28 20:00
---

xmrmfjj2[^1] was tricked into paying an exorbitant 19.73 XMR transaction fee by a malicious Monero remote node:

> 391d2a8c6d34267d673f06e631e631ea213180f4df7193a37091d540be92a605 transaction posted 2.5 xmr commission 19.73xmr why such a commission? how to return 19.73 help I use Monero GUI Wallet[^2]

The transaction was sent with an unspecified version of the official Monero GUI wallet, most probably running in *Simple mode* (connected to a random remote node), and it was mined by Solopool[^3] in block 2610570[^4].

selsta[^5] has opened a PR (#3897[^6]) that implements a warning for future users whenever the remote node sets a high fee.

![selsta PR](/assets/img/stories/selsta-3897.png)

Note that this pull request is only a *quick fix*:

> The only long term solution will be to remove the remote node scanner from simple mode and use hardcoded trusted community nodes. (selsta)[^7]

This is not the first time something like this happens. In January, PacificNWVet paid a 3.93 XMR fee for transferring 0.34 XMR. That particular user was lucky to have the full amount lost in fees covered by the Monero community, as previously reported[^8].

It is unclear how and if xmrmfjj2 will be able to recover the funds, as the block reward was probably distributed to miners by now and the pool admin has not yet replied.

## Tips

- always verify the fee before sending any transaction
- connect to a trusted remote node, switch nodes (or run your own node) 
- always use the latest wallet version

*This report will be updated when new information is available.*

---

[^1]: https://github.com/xmrmfjj2
[^2]: [https://github.com/monero-project/monero/issues/8298](https://github.com/monero-project/monero/issues/8298){:target="_blank"}{:rel="nofollow"}
[^3]: https://xmr.solopool.org/
[^4]: https://xmrchain.net/block/2610570
[^5]: https://github.com/selsta
[^6]: [https://github.com/monero-project/monero-gui/pull/3897](https://github.com/monero-project/monero-gui/pull/3897){:target="_blank"}{:rel="nofollow"}
[^7]: https://github.com/monero-project/monero-gui/pull/3897#issuecomment-1111267136
[^8]: [/pacificnwvet-pays-3.93-xmr-fee-0.34-xmr-transaction](/pacificnwvet-pays-3.93-xmr-fee-0.34-xmr-transaction)
