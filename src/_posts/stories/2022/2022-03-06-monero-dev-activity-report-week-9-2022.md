---
layout: post
category: story
title: "Monero Dev Activity Report - Week 9 2022: 17 PRs, 8 Issues"
description: "This weekly report aims to provide a big picture view of Monero development activity, increase community support for existing devs and, hopefully, encourage new contributions."
tags: dev
image: 
date: 2022-03-06 21:00
---

This weekly report aims to provide a big picture view of Monero development activity, increase community support for existing devs and, hopefully, encourage new contributions.


## 1 - PRs (17, 10:1:6)

Opened (10)

`monero-project/monero`:

- **#8207[^1]** CMake: Add missing headers via monero_find_all_headers macro (mj-xmr)
- **#8205[^2]** Compil. time: cryptonote_core minus portable_storage header (mj-xmr)
- **#8203[^3]** multisig: add key exchange round booster (UkoeHB)
- **#8202[^4]** Daemon: Store blockchain in '~/.local/share/bitmonero' by default (mj-xmr)
- **#8200[^5]** Compil. time: http_client.h -> abstract_http_client.h (mj-xmr)
- **#8197[^6]** Copyright: Update to 2022 (mj-xmr)
- **#8196[^7]** [release-v0.17] wallet2: update stagenet rollback blocks (selsta)
- **#8195[^8]** wallet2: update stagenet rollback blocks (selsta)

`monero-project/monero-gui`:

- **#3849[^9]** libwalletqt: fix typo in type (selsta)
- **#3846[^10]** Wizard: fix stagenet approx blockheight (selsta)

Closed (1)

`monero-project/monero`:

- **#8201[^11]** Add Ninja to list of Mingw dependencies in README.md (jeffro256)

`monero-project/monero-gui`: None

Merged (6)

`monero-project/monero`: None

`monero-project/monero-gui`:

- **#3841[^12]** workflows: fix windows build error (reemuru)
- **#3838[^13]** settings: bind return key after password change (reemuru)
- **#3832[^14]** Adding translations from Weblate (Monero-Weblate)
- **#3831[^15]** bug: reset wallet path on network change (reemuru)
- **#3828[^16]** Advanced: ReserveProof: Add support for reserve proof (reemuru)
- **#3825[^17]** WizardRestoreWallet4, WizardCreateWallet4: disable double-click on "Create wallet" button (rating89us)


## 2 - ISSUES (8, 6:2)

Opened (6)

`monero-project/monero`:

- **#8206[^18]** unit_tests node_server.bind_same_p2p_port FAILED (BebeSparkelSparkel)
- **#8204[^19]** How to simulate a TXID for multiple UTXO transaction (EWIT521)
- **#8199[^20]** ZMQ DESTROYED by p2pool daemon. (Gingeropolous)

`monero-project/monero-gui`:

- **#3850[^21]** Window resizing issue when running dual monitors on a PC (geonic1)
- **#3848[^22]** Wallet.cpp error on windows build (reemuru)
- **#3847[^23]** Monero Blockchain download from gui (advanced) (Kekko93)

Closed (2)

`monero-project/monero`:

- **#8208[^24]** SSD Bottleneck and wear with monolithic file. (ThomasAn73)
- **#8198[^25]** Payment never received (similar to issue #8134) (ikseles)

`monero-project/monero-gui`: None


That's it for this week's dev activity report. I will try and publish one every Sunday. Let me know if I missed anything or if you want to see any other statistics/repos included in future reports. Feedback/edits: @ [/about](/about).

**-3RA**

---

[^1]: https://github.com/monero-project/monero/pull/8207
[^2]: https://github.com/monero-project/monero/pull/8205
[^3]: https://github.com/monero-project/monero/pull/8203
[^4]: https://github.com/monero-project/monero/pull/8202
[^5]: https://github.com/monero-project/monero/pull/8200
[^6]: https://github.com/monero-project/monero/pull/8197
[^7]: https://github.com/monero-project/monero/pull/8196
[^8]: https://github.com/monero-project/monero/pull/8195
[^9]: https://github.com/monero-project/monero-gui/pull/3849
[^10]: https://github.com/monero-project/monero-gui/pull/3846
[^11]: https://github.com/monero-project/monero/pull/8201
[^12]: https://github.com/monero-project/monero-gui/pull/3841
[^13]: https://github.com/monero-project/monero-gui/pull/3838
[^14]: https://github.com/monero-project/monero-gui/pull/3832
[^15]: https://github.com/monero-project/monero-gui/pull/3831
[^16]: https://github.com/monero-project/monero-gui/pull/3828
[^17]: https://github.com/monero-project/monero-gui/pull/3825
[^18]: https://github.com/monero-project/monero/issues/8206
[^19]: https://github.com/monero-project/monero/issues/8204
[^20]: https://github.com/monero-project/monero/issues/8199
[^21]: https://github.com/monero-project/monero-gui/issues/3850
[^22]: https://github.com/monero-project/monero-gui/issues/3848
[^23]: https://github.com/monero-project/monero-gui/issues/3847
[^24]: https://github.com/monero-project/monero/issues/8208
[^25]: https://github.com/monero-project/monero/issues/8198
