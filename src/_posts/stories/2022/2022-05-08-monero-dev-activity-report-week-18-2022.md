---
layout: post
category: story
title: "Monero Dev Activity Report - Week 18 2022: 13 PRs, 11 Issues"
description: "This weekly report aims to provide a big picture view of Monero development activity, increase community support for existing devs and, hopefully, encourage new contributions."
tags: dev
image: 
---

This weekly report aims to provide a big picture view of Monero development activity, increase community support for existing devs and, hopefully, encourage new contributions.

## 1 - PRs (13, 13:0:0)

Opened (13)

`monero-project/monero`:

- **#8307[^1]** Remove src/serialization/list.h (jeffro256)
- **#8308[^2]** wallet2: fix a couple unused variable warnings (selsta)
- **#8312[^3]** gitian: add ARM64 Darwin support (hyc)
- **#8315[^4]** Give better error messages when missing SSL files (jeffro256)
- **#8317[^5]** wallet_rpc_server: add daemon connection check (reemuru)
- **#8318[^6]** utils: delete outdated windows build script (selsta)
- **#8319[^7]** update readme Scheduled upgrades section (Gingeropolous)

`monero-project/monero-gui`:

- **#3908[^8]** workflows: add caching for docker android (selsta)
- **#3910[^9]** History: fix payment proof button (reemuru)
- **#3913[^10]** p2pool: fix monerod sometimes restarting with invalid arguments (devhyper)
- **#3914[^11]** main: disable setting -platformpluginpath (selsta)
- **#3915[^12]** qt: replace QRegExp with QRegularExpression (selsta)
- **#3916[^13]** qt: remove QTextCodec (selsta)

Closed (0)

`monero-project/monero`: none

`monero-project/monero-gui`: none

Merged (0)

`monero-project/monero`: none

`monero-project/monero-gui`: none

## 2 - ISSUES (11, 6:5)

Opened (6)

`monero-project/monero`: 

- **#8310[^14]** Update hardforks.cpp (lubomr)
- **#8311[^15]** get_transactions returns as_hex: "" for miner transactions (kayabaNerve)
- **#8314[^16]** Support checking if wallet rpc is connected to daemon (woodser)
- **#8316[^17]** [bug] - Set daemon allows any address (reemuru)

`monero-project/monero-gui`: 

- **#3909[^18]** Bug v0.17.3.2 Generate payment proof button (tczee36)
- **#3911[^19]** monerod second instance started by GUI (MainTsk)

Closed (5)

`monero-project/monero`:

- **#8313[^20]** Bug v0.17.3.2 Generate payment proof button - non responsive (tczee36)
- **#8309[^21]** v0.17.3.2 does not compile on OpenBSD 7.1 (random-xmr-user)

`monero-project/monero-gui`: 

- **#3579[^22]** Transfer: error when signing tx file (offline transaction signing) (rating89us)
- **#2005[^23]** Titlebar: create Lock wallet button (rating89us)
- **#3912[^24]** GUI wallet synced with daemon; funds not appearing (anon74652393854769423587)

That's it for this week's dev activity report. I will try and publish one every Sunday. Let me know if I missed anything or if you want to see any other statistics/repos included in future reports. Feedback/edits: @ [/about](/about).

Previous reports are listed in the [[dev]](/tag/dev) section. 

**-3RA**

---

[^1]: https://github.com/monero-project/monero/pull/8307
[^2]: https://github.com/monero-project/monero/pull/8308
[^3]: https://github.com/monero-project/monero/pull/8312
[^4]: https://github.com/monero-project/monero/pull/8315
[^5]: https://github.com/monero-project/monero/pull/8317
[^6]: https://github.com/monero-project/monero/pull/8318
[^7]: https://github.com/monero-project/monero/pull/8319

[^8]: https://github.com/monero-project/monero-gui/pull/3908
[^9]: https://github.com/monero-project/monero-gui/pull/3910
[^10]: https://github.com/monero-project/monero-gui/pull/3913
[^11]: https://github.com/monero-project/monero-gui/pull/3914
[^12]: https://github.com/monero-project/monero-gui/pull/3915
[^13]: https://github.com/monero-project/monero-gui/pull/3916

[^14]: https://github.com/monero-project/monero-gui/issues/8310
[^15]: https://github.com/monero-project/monero-gui/issues/8311
[^16]: https://github.com/monero-project/monero-gui/issues/8314
[^17]: https://github.com/monero-project/monero-gui/issues/8316

[^18]: https://github.com/monero-project/monero/issues/3909
[^19]: https://github.com/monero-project/monero/issues/3911

[^20]: https://github.com/monero-project/monero/issues/8313
[^21]: https://github.com/monero-project/monero/issues/8309

[^22]: https://github.com/monero-project/monero-gui/issues/3579
[^23]: https://github.com/monero-project/monero-gui/issues/2005
[^24]: https://github.com/monero-project/monero-gui/issues/3912

