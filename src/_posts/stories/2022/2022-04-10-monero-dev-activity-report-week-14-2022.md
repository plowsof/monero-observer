---
layout: post
category: story
title: "Monero Dev Activity Report - Week 14 2022: 31 PRs, 39 Issues"
description: "This weekly report aims to provide a big picture view of Monero development activity, increase community support for existing devs and, hopefully, encourage new contributions."
tags: dev
image: 
date: 2022-04-10 20:00
last_modified_at: 2022-04-17
---

This weekly report aims to provide a big picture view of Monero development activity, increase community support for existing devs and, hopefully, encourage new contributions.

## 1 - PRs (31, 13:2:16)

Opened (13)

`monero-project/monero`:

- **#8239[^1]** Added support for Ledger Nano S Plus [release-v0.17] (selsta)
- **#8240[^2]** randomx: update submodule (selsta)
- **#8241[^3]** randomx: update submodule [release-v0.17] (selsta)
- **#8245[^4]** simplewallet: fix integrated_address output string (selsta)
- **#8246[^5]** Makefile: fix spelling of CMAKE_BUILD_TYPE value (selsta)
- **#8247[^6]** readme: small fixes (hinto-janaiyo)
- **#8248[^7]** Remove serialization/enableable (jeffro256)
- **#8249[^8]** Remove /include (jeffro256)
- **#8250[^9]** Remove src/platform (jeffro256)
- **#8254[^10]** wallet2: use BP+ for cold signing (moneromooo-monero)

`monero-project/monero-gui`:

- **#3878[^11]** wizard: redesign seed page (selsta)
- **#3879[^12]** cmake: bump windows deploy lib versions, update workflows (selsta)
- **#3883[^13]** Makefile: fix spelling of CMAKE_BUILD_TYPE value (selsta)

Closed (2)

`monero-project/monero`: none

`monero-project/monero-gui`: 

- **#3667[^14]** wizard: move mnemonic seed into a separate screen (rating89us)
- **#3853[^15]** Update languages.xml (whirlwind110)

Merged (16)

`monero-project/monero`: 

- **#8166[^16]** support authentication in monero-wallet-rpc set_daemon (woodser)
- **#8177[^17]** simplewallet: rename duplicate amount headers for clarity (woodser)
- **#8179[^18]** wallet2: decrease the amount of data exchanged for output export (moneromooo-monero)
- **#8180[^19]** simplewallet: add option for exporting tx keys (reemuru)
- **#8195[^20]** wallet2: update stagenet rollback blocks (selsta)
- **#8196[^21]** [release-v0.17] wallet2: update stagenet rollback blocks (selsta)
- **#8197[^22]** Copyright: Update to 2022 (mj-xmr)
- **#8205[^23]** Compil. time: cryptonote_core minus portable_storage header (mj-xmr)
- **#8212[^24]** Remove footgun doc comment in miner TX validation (kayabaNerve)
- **#8213[^25]** wallet_rpc_server: fix make_integrated_address with no payment id (moneromooo-monero)
- **#8215[^26]** wallet_rpc_server: support regex for tags in get_accounts (reemuru)
- **#8222[^27]** [release-v0.17] replace erciccione's seednode with one on haveno's infrastructure (erciccione)
- **#8223[^28]** Eliminate dependence on boost::interprocess (jeffro256)
- **#8227[^29]** [release-v0.17] Don't require --rpc-login with --rpc-access-control-origins (jeffro256)
- **#8228[^30]** Remove dead code from parserse_base_utils and fix unit tests (jeffro256)
- **#8242[^31]** tests: integrated_address: remove missing payment id assertion (reemuru)

`monero-project/monero-gui`: None


## 2 - ISSUES (39, 5:34)

Opened (5)

`monero-project/monero`: 

- **#8237[^32]** Monero Multisig for HF (UkoeHB)
- **#8238[^33]** monerod Segmentation fault in libzmq.so (othello777)
- **#8251[^34]** Feature: resubmit a failed tx from the wallet (j-berman)
- **#8253[^35]** Is there any method for monero wallet rpc that returns transactions on ALL subaccounts? (Ext7)

`monero-project/monero-gui`:

- **#3884[^36]** Operation not permitted while trying to run monerod (v0.17.3.1) (Linux) (manuel-arguelles)

Closed (34)

`monero-project/monero`:

- **#8231[^37]** Can I contribute in rust? (daniel-brenot)
- **#8234[^38]** Compilation failure of v0.17.3.0 with OpenBSD 7 on RiscV-64 (antanst)
- **#8243[^39]** Starting wallet RPC server - stuck (martinoshub)
- **#8244[^40]** Question: Seems I send monero to two address in a single payment (ycMia)
- **#8252[^41]** GUI wallet is inaccessible with voiceover on Mac (demhademha)
- **#8176[^42]** Feature request: optionally export tx_keys with export_transfer (SamsungGalaxyPlayer)
- **#8214[^43]** Regexp support for listing accounts (by moneromooo-monero)
- **#844[^44]** Tighten up torsocks usage recommendations in README.md (iamsmooth)
- **#1052[^45]** Simplewallet problem with send (AJIekceu4)
- **#2204[^46]** [Feature Request] Remote node service advertising and remote refreshing through daemon (Gingeropolous)
- **#3056[^47]** Cross-compiling fails running generate_translations_header (danrmiller)
- **#3059[^48]** RPC: Wrongly formatted RFC 2616/2617 header (onodera-punpun)
- **#3223[^49]** macOS: readline broken with torsocks (Ctrl-C is ignored) (heptathlon)
- **#3319[^50]** [bug] Cold Signing not possible between 64-bit (ubuntu) and armv7(ubuntu) (nasaWelder)
- **#3742[^51]** Error: Couldn't connect to daemon (after importing blockchain.raw) (WPFilmmaker)
- **#3265[^52]** [Fork Attack Mitigation] add sweep_all_fork that accepts two destination addresses (nasaWelder)
- **#3826[^53]** Fail to build on PPC64 (hegjon)
- **#3905[^54]** Taking too long to make a cold sign due to export_outputs file size is big if there are too many outputs. (zhongqiuwood)
- **#3996[^55]** We need a note on spinning drives (littleblackfish)
- **#4140[^56]** monero wallet rpc shows unlocked balance as 0 and thus does not let to transfer monero testnet coins.While monero cli shows and lets transfer monero (alishaagupta)
- **#4213[^57]** Re-enumerating devices while monerod running with --data-dir on a USB drive causes the blockchain to become corrupt. (malixg)
- **#4285[^58]** show_transfers bug (carrie143)
- **#4690[^59]** Building on Docker with BUILD_SHARED_LIBS=ON: error: dereferencing pointer to incomplete type 'EVP_MD_CTX {aka struct evp_md_ctx_st}' (whidrasl)
- **#3951[^60]** CLI won't prompt for password (krtschmr)
- **#5262[^61]** Buss error (core dumped) while upgrading database (zahyur)
- **#5914[^62]** Setting up a wallet with a full node and tor should be easier (kpcyrd)
- **#6292[^63]** CLI prompt showing password in clear (dalecooper)
- **#6186[^64]** xmr rpc 401 Unauthorized (NoBugBoy)
- **#6400[^65]** make failed on centos7(call to non-constexpr function) (liuxh-go)


`monero-project/monero-gui`: 

- **#3880[^66]** Had bluescreen while syncing blocks MONERO GUI (blockchain on pc) (Kekko93)
- **#3881[^67]** Error: Couldn't connect to daemon (Kekko93)
- **#3882[^68]** auto changes all address book descriptions to the last one (alias-bitsignal)
- **#3855[^69]** Error compiling for Windows (tjmitchem)
- **#3847[^70]** Monero Blockchain download from gui (advanced) (Kekko93)




That's it for this week's dev activity report. I will try and publish one every Sunday. Let me know if I missed anything or if you want to see any other statistics/repos included in future reports. Feedback/edits: @ [/about](/about).

Previous reports are listed in the [[dev]](/tag/dev) section. 

**-3RA**

---

**Update: added missing Issues (Closed).**

---

[^1]: https://github.com/monero-project/monero/pull/8239
[^2]: https://github.com/monero-project/monero/pull/8240
[^3]: https://github.com/monero-project/monero/pull/8241
[^4]: https://github.com/monero-project/monero/pull/8245
[^5]: https://github.com/monero-project/monero/pull/8246
[^6]: https://github.com/monero-project/monero/pull/8247
[^7]: https://github.com/monero-project/monero/pull/8248
[^8]: https://github.com/monero-project/monero/pull/8249
[^9]: https://github.com/monero-project/monero/pull/8250
[^10]: https://github.com/monero-project/monero/pull/8254

[^11]: https://github.com/monero-project/monero-gui/pull/3878
[^12]: https://github.com/monero-project/monero-gui/pull/3879
[^13]: https://github.com/monero-project/monero-gui/pull/3883

[^14]: https://github.com/monero-project/monero-gui/pull/3667
[^15]: https://github.com/monero-project/monero-gui/pull/3853

[^16]: https://github.com/monero-project/monero/pull/8166
[^17]: https://github.com/monero-project/monero/pull/8177
[^18]: https://github.com/monero-project/monero/pull/8179
[^19]: https://github.com/monero-project/monero/pull/8180
[^20]: https://github.com/monero-project/monero/pull/8195
[^21]: https://github.com/monero-project/monero/pull/8196
[^22]: https://github.com/monero-project/monero/pull/8197
[^23]: https://github.com/monero-project/monero/pull/8205
[^24]: https://github.com/monero-project/monero/pull/8212
[^25]: https://github.com/monero-project/monero/pull/8213
[^26]: https://github.com/monero-project/monero/pull/8215
[^27]: https://github.com/monero-project/monero/pull/8222
[^28]: https://github.com/monero-project/monero/pull/8223
[^29]: https://github.com/monero-project/monero/pull/8227
[^30]: https://github.com/monero-project/monero/pull/8228
[^31]: https://github.com/monero-project/monero/pull/8242

[^32]: https://github.com/monero-project/monero/issues/8237
[^33]: https://github.com/monero-project/monero/issues/8238
[^34]: https://github.com/monero-project/monero/issues/8251
[^35]: https://github.com/monero-project/monero/issues/8253

[^36]: https://github.com/monero-project/monero-gui/issues/3884

[^37]: https://github.com/monero-project/monero/issues/8231
[^38]: https://github.com/monero-project/monero/issues/8234
[^39]: https://github.com/monero-project/monero/issues/8243
[^40]: https://github.com/monero-project/monero/issues/8244
[^41]: https://github.com/monero-project/monero/issues/8252

[^42]: https://github.com/monero-project/monero/issues/8176
[^43]: https://github.com/monero-project/monero/issues/8214
[^44]: https://github.com/monero-project/monero/issues/844
[^45]: https://github.com/monero-project/monero/issues/1052
[^46]: https://github.com/monero-project/monero/issues/2204
[^47]: https://github.com/monero-project/monero/issues/3056
[^48]: https://github.com/monero-project/monero/issues/3059
[^49]: https://github.com/monero-project/monero/issues/3223
[^50]: https://github.com/monero-project/monero/issues/3319
[^51]: https://github.com/monero-project/monero/issues/3742
[^52]: https://github.com/monero-project/monero/issues/3265
[^53]: https://github.com/monero-project/monero/issues/3826
[^54]: https://github.com/monero-project/monero/issues/3905
[^55]: https://github.com/monero-project/monero/issues/3996
[^56]: https://github.com/monero-project/monero/issues/4140
[^57]: https://github.com/monero-project/monero/issues/4213
[^58]: https://github.com/monero-project/monero/issues/4285
[^59]: https://github.com/monero-project/monero/issues/4690
[^60]: https://github.com/monero-project/monero/issues/3951
[^61]: https://github.com/monero-project/monero/issues/5262
[^62]: https://github.com/monero-project/monero/issues/5914
[^63]: https://github.com/monero-project/monero/issues/6292
[^64]: https://github.com/monero-project/monero/issues/6186
[^65]: https://github.com/monero-project/monero/issues/6400

[^66]: https://github.com/monero-project/monero-gui/issues/3880
[^67]: https://github.com/monero-project/monero-gui/issues/3881
[^68]: https://github.com/monero-project/monero-gui/issues/3882

[^69]: https://github.com/monero-project/monero-gui/issues/3855
[^70]: https://github.com/monero-project/monero-gui/issues/3847
