---
layout: post
category: story
title: libwallet viewkey-based background refresh enhancenement to significantly reduce wallet sync time
description: "The Monero community is considering a libwallet viewkey-based background refresh enhancenement that should significantly reduce wallet sync time."
tags: [bounties, dev]
image: 
date: 2021-11-26 20:00
---

The Monero community is discussing a potential libwallet viewkey-based background refresh enhancenement[^1] that should significantly reduce wallet sync time.

Howard Chu[^2] proposed[^3] starting with the addition of a `background-sync-cache` that is separate from the main wallet cache and which has its own secret key:

> [..] used to perform refreshes with the wallet viewkey while the main wallet is idle/off. The point is to allow the wallet to stay sync'd with the blockchain without leaving the private spendkey exposed or leaving the main wallet cache in decrypted state.

Justin Ehrenhofer[^4] suggested[^5] an even more ambitious approach, which would work even for powered off devices, by allowing remote nodes to function as lightweight servers:

> The ideal for almost all wallets is to be able to send the view key to a chosen remote node, which can then act as a lightweight server and scan all blocks on the server side.

If this gets implemented in the core Monero libwallet source, it will probably be included by other wallets like Monerujo and Cake wallet. 

There are currently 3 relevant bounties[^6]'[^7]'[^8] on Monero.social, but the one posted by CryptoGrampy[^9] for the official Monero software has priority:

```
Total Bounty: 0.1 XMR (to date)
```

### Minimum requirements

- Code is open-source
- Code is submitted to the Monero repo as a pull-request (https://github.com/monero-project/monero/pulls)
- Work with Monero devs and mobile wallet devs (Monerujo, Cake, etc) to determine agreed-upon solution
- Pull request properly improves wallet sync time
- Pull request is accepted into Monero's code base after review

To start working on the project yourself, you should make your intentions public by posting a comment in the bounty's thread[^6].

Alternatively you can contribute some XMR to the bounty address posted by the *Monero Bounties Bot*.

As previously reported[^10], j-berman[^11] has already submitted a pull request (PR #8061[^12]) that aims to decrease wallet sync times. This should be included in the next Monero v0.18.0 release (HF v15[^13]).

---

[^1]: [https://github.com/monero-project/monero/issues/8082](https://github.com/monero-project/monero/issues/8082){:target="_blank"}{:rel="nofollow"}
[^2]: https://github.com/hyc
[^3]: https://github.com/monero-project/monero/issues/8082#issue-1064233757
[^4]: https://github.com/SamsungGalaxyPlayer
[^5]: https://github.com/monero-project/monero/issues/8082#issuecomment-980370275
[^6]: [https://bounties.monero.social/posts/41/](https://bounties.monero.social/posts/41/){:target="_blank"}
[^7]: https://bounties.monero.social/posts/9/
[^8]: https://bounties.monero.social/posts/10/
[^9]: https://github.com/CryptoGrampy
[^10]: [/proposal-decrease-wallet-sync-times-fueled-community-bounty/](/proposal-decrease-wallet-sync-times-fueled-community-bounty/)
[^11]: https://github.com/j-berman
[^12]: https://github.com/monero-project/monero/pull/8061
[^13]: [/monero-hard-fork-v15-planned-early-spring-2022/](/monero-hard-fork-v15-planned-early-spring-2022/)
