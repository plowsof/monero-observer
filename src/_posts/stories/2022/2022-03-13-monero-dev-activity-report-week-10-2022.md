---
layout: post
category: story
title: "Monero Dev Activity Report - Week 10 2022: 14 PRs, 10 Issues"
description: "This weekly report aims to provide a big picture view of Monero development activity, increase community support for existing devs and, hopefully, encourage new contributions."
tags: dev
image: 
date: 2022-03-13 20:30
---

This weekly report aims to provide a big picture view of Monero development activity, increase community support for existing devs and, hopefully, encourage new contributions.

## 1 - PRs (14, 11:2:1)

Opened (11)

`monero-project/monero`:

- **#8211[^1]** EPEE Cleanup Reorganized (jeffro256)
- **#8212[^2]** Remove footgun doc comment in miner TX validation (kayabaNerve)
- **#8213[^3]** wallet_rpc_server: fix make_integrated_address with no payment id (moneromooo-monero)
- **#8215[^4]** wallet_rpc_server: support regex for tags in get_accounts (reemuru)
- **#8216[^5]** replace erciccione's seednode with one on haveno's infrastructure (erciccione)

`monero-project/monero-gui`:

- **#3851[^6]** Doc: Minimize boost deps in README.md (mj-xmr)
- **#3852[^7]** Make fiat price APIs more flexible (elibroftw)
- **#3853[^8]** Update languages.xml (whirlwind110)
- **#3858[^9]** CMake: clearer sep. between the library and executable code (mj-xmr)
- **#3859[^10]** SettingsWallet: lock wallet on demand  (reemuru)
- **#3860[^11]** RemoteNodeDialog: bind ok to return key (reemuru)

Closed (2)

`monero-project/monero`:

- **#8175[^12]** Epee Cleanup (jeffro256)

`monero-project/monero-gui`: 

- **#2995[^13]** history: change sent transaction dot color from orange to red (rating89us)

Merged (1)

`monero-project/monero`: None

`monero-project/monero-gui`:

- **#3849[^14]** libwalletqt: fix typo in type (selsta)



## 2 - ISSUES (10, 6:4)

Opened (6)

`monero-project/monero`:

- **#8210[^15]** FreeBSD "Listen queue overflow" issues (camberkenpas)
- **#8204[^16]** Regexp support for listing accounts (moneromooo-monero)
- **#8199[^17]** We forked Monero - Cannot send coins (underthetablecoin)

`monero-project/monero-gui`:

- **#3855[^18]** Error compiling for Windows (tjmitchem)
- **#3856[^19]** Cannot build just "monero-wallet-gui" target, as it has strong dependency on target "daemon" (jjakob)
- **#3857[^20]** [Feature] Lock Wallet & Bind it with Ctrl + L (elibroftw)

Closed (4)

`monero-project/monero`:

- **#8206[^21]** unit_tests node_server.bind_same_p2p_port FAILED (BebeSparkelSparkel)
- **#8209[^22]** Fresh fullnode does not sync (taoeffect)

`monero-project/monero-gui`: 

- **#3848[^23]** Wallet.cpp error on windows build (reemuru)
- **#3854[^24]** Daemon failed to start - Linux Mint (harrwester)



That's it for this week's dev activity report. I will try and publish one every Sunday. Let me know if I missed anything or if you want to see any other statistics/repos included in future reports. Feedback/edits: @ [/about](/about).

Previous reports are listed in the [[dev]](/tag/dev) section. 

**-3RA**

---

[^1]: https://github.com/monero-project/monero/pull/8211
[^2]: https://github.com/monero-project/monero/pull/8212
[^3]: https://github.com/monero-project/monero/pull/8213
[^4]: https://github.com/monero-project/monero/pull/8215
[^5]: https://github.com/monero-project/monero/pull/8216
[^6]: https://github.com/monero-project/monero/pull/3851
[^7]: https://github.com/monero-project/monero/pull/3852
[^8]: https://github.com/monero-project/monero/pull/3853
[^9]: https://github.com/monero-project/monero-gui/pull/3858
[^10]: https://github.com/monero-project/monero-gui/pull/3859
[^11]: https://github.com/monero-project/monero/pull/3860
[^12]: https://github.com/monero-project/monero-gui/pull/8175
[^13]: https://github.com/monero-project/monero-gui/pull/2995
[^14]: https://github.com/monero-project/monero-gui/pull/3849
[^15]: https://github.com/monero-project/monero-gui/pull/8210
[^16]: https://github.com/monero-project/monero-gui/pull/8204
[^17]: https://github.com/monero-project/monero-gui/pull/8199
[^18]: https://github.com/monero-project/monero/issues/3855
[^19]: https://github.com/monero-project/monero/issues/3856
[^20]: https://github.com/monero-project/monero/issues/3857
[^21]: https://github.com/monero-project/monero-gui/issues/8206
[^22]: https://github.com/monero-project/monero-gui/issues/8209
[^23]: https://github.com/monero-project/monero-gui/issues/3848
[^24]: https://github.com/monero-project/monero/issues/3854
