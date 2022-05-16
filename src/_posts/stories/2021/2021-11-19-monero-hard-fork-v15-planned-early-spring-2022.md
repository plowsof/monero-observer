---
layout: post
category: story
title: Monero hard-fork v15 planned for early Spring 2022
description: "The next Monero hard-fork (version 15) for release v0.18.0 is planned for early Spring 2022."
tags: [dev, pinned]
image: 
date: 2021-11-19 20:00
---

The next Monero hard-fork (version 15)[^1] for release v0.18.0[^2] is planned for early Spring 2022[^3]:

> [..] the tentative plan would be an early Spring hard-fork, i.e. February or March of 2022.

It is worth noting that both Triptych and Seraphis are off the table for this network upgrade.

### Primary features included

- Ring-size increase from 11 to 16 (#79[^4])
- View tags by @jberman (#8061[^5])
- Fee changes from @articmine (#7819[^6])
- Bulletproofs+ (#7170[^7])

### Potential features

- Output binning changes by @jberman (#88[^8])
- Multisig refactor and vulnerability fix by @UkoeHB (#7877[^9])
- Daemon connection fixes (#7760[^10])

Before the HF happens, there are a number of items that have to be completed first (RELEASE_CHECKLIST[^11]): a security audit, code audit, Ledger/Trezor integration, send notifications to wallets, exchanges, mining pools and 3rd party payment processors and post release announcements.

---

[^1]: https://github.com/monero-project/monero#scheduled-software-upgrades
[^2]: https://github.com/monero-project/meta/issues/623
[^3]: [https://github.com/monero-project/meta/issues/630](https://github.com/monero-project/meta/issues/630){:target="_blank"}{:rel="nofollow"}
[^4]: https://github.com/monero-project/research-lab/issues/79
[^5]: https://github.com/monero-project/monero/pull/8061
[^6]: https://github.com/monero-project/monero/pull/7819
[^7]: https://github.com/monero-project/monero/pull/7170
[^8]: https://github.com/monero-project/research-lab/issues/88
[^9]: https://github.com/monero-project/monero/pull/7877
[^10]: https://github.com/monero-project/monero/pull/7760
[^11]: https://github.com/monero-project/monero/blob/master/docs/RELEASE_CHECKLIST.md
