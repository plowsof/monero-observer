---
layout: post
category: story
title: "Monero Dev Activity Report - Week 11 2022: 25 PRs, 38 Issues"
description: "This weekly report aims to provide a big picture view of Monero development activity, increase community support for existing devs and, hopefully, encourage new contributions."
tags: dev
image: 
date: 2022-03-20 21:00
---

This weekly report aims to provide a big picture view of Monero development activity, increase community support for existing devs and, hopefully, encourage new contributions.

## 1 - PRs (25, 5:2:18)

Opened (5)

`monero-project/monero`:

- **#8220[^1]** multisig: add post-kex verification round (UkoeHB)
- **#8222[^2]** [release-v0.17] replace erciccione's seednode with one on haveno's infrastructure (erciccione)
- **#8223[^3]** Eliminate dependence on boost::interprocess (jeffro256)

`monero-project/monero-gui`:

- **#3868[^4]** StandardDropdown: Add Flickable and ScrollBar to droplist (reemuru)
- **#3869[^5]** TitleBar: Remove lock icon on essentials display (reemuru)

Closed (2)

`monero-project/monero`: None

`monero-project/monero-gui`: 

- **#3862[^6]** Added support for more fiat currencies. (reemuru)
- **#3863[^7]** AddressBook: fix index 0 description bug (reemuru)

Merged (18)

`monero-project/monero`: 

- **#8154[^8]** Balance includes unconfirmed payments (woodser)
- **#8158[^9]** Balance includes unconfirmed transfers to self (woodser)
- **#8159[^10]** Balance includes unconfirmed transfers to self (woodser)
- **#8169[^11]** rpc: add explicit restricted flag to /get_info (tobtoht)
- **#8170[^12]** systemd: remove outdated torsocks example (selsta)
- **#8186[^13]** Undefined behaviour fixes (SChernykh)
- **#8187[^14]** Fixes: Don't require --rpc-login with --rpc-access-control-origins (jeffro256)
- **#8190[^15]** multisig key exchange update and refactor - release-v0.17 (UkoeHB)
- **#8216[^16]** replace erciccione's seednode with one on haveno's infrastructure (erciccione)
- **#7675[^17]** workflows: don't build PRs if only docs and READMEs are being changed (erciccione)


`monero-project/monero-gui`:

- **#3470[^18]** cmake: remove unneeded monero_gui_add_library() (selsta)
- **#3719[^19]** cmake: don't print verbose make (selsta)
- **#3720[^20]** cmake: remove including non-existent directory (selsta)
- **#3851[^21]** Doc: Minimize boost deps in README.md (mj-xmr)
- **#3859[^22]** SettingsWallet: lock wallet on demand (reemuru)
- **#3860[^23]** RemoteNodeDialog: bind ok to return key (reemuru)
- **#3862[^24]** Transfer: fix offline signing (reemuru)
- **#3865[^25]** AddressBook: fix adding new entry (selsta)



## 2 - ISSUES (38, 2:36)

Opened (2)

`monero-project/monero`: None

`monero-project/monero-gui`:

- **#3864[^26]** StandardDropdown is not Scrollable (elibroftw)
- **#3867[^27]** No way to exit out of Confirm Send Modal (elibroftw)

Closed (36)

`monero-project/monero`:

- **#60[^28]** Implement support for connecting through proxy (Jojatekok)
- **#1520[^29]** FreeBSD Port (emc2)
- **#2522[^30]** monerod_sync_ERROR (dranogy)
- **#3330[^31]** Input/Output error - Core Dumped in VBox (jodobear)
- **#3234[^32]** Problems at read: Operation canceled with local node (cialu)
- **#3572[^33]** Mingw64 build warning (Keksov)
- **#3537[^34]** linking error bin/monero-wallet-cli.exe windows 7 monero v0.12 (blockchainbuzz)
- **#3425[^35]** Hosting seed node (fengshuicoin)
- **#3394[^36]** Error: failed to generate new wallet: failed to save file "./home/wallet1.keys" (kevingwang)
- **#3415[^37]** monero-wallet-cli 0.11.1 segfaults with "Resource temporarily unavailable" when refreshing (emesik)
- **#3513[^38]** Mnemonic seed restores to wrong address with early blockchain (HuangYuSan)
- **#3409[^39]** Monero blocks indefinitely when sweeping unmixable outputs (lomacks)
- **#3519[^40]** We need RawImport for Testnet (krtschmr)
- **#3845[^41]** Daemon hangs after "DB resize needed" on ARM Debian (Lafudoci)
- **#4497[^42]** Update version with every tag (normoes)
- **#4462[^43]** ERROR net.http src/rpc/core_rpc_server.h:84 Failed to on_get_blocks() (jdscott0)
- **#3874[^44]** monerod can't restart after power down (AlexVN74)
- **#3949[^45]** monerod crashing when using with the USX GUI wallet (ManfredKarrer)
- **#4141[^46]** Monero wallet cli shows balance 29 and unlocked balance 5, while wallet rpc call shows balance 5 and unlocked balance 0. (alishaagupta)
- **#4039[^47]** monero-wallet-rpc does not like to connect to Tor hidden services (moneromooo-monero)
- **#5233[^48]** Problem with monero-wallet-cli.exe (angryFlo)
- **#5644[^49]** monerod: Failed to delete transaction prunable data (ukfhVp0zms)
- **#6323[^50]** Manually adding sub addresses to wallet (godfuture)
- **#6391[^51]** There is a problem in sync during monerod. Who can give me some suggestions? (xcoin-dev)
- **#7259[^52]** Segmentation error when syncing Armv8 Rock64 (SomaticFanatic)
- **#8221[^53]** Monero GUI Wallet download issue (Vacman)
- **#8073[^54]** Add change output to wallet balance immediately (woodser)


`monero-project/monero-gui`: 

- **#3861[^55]** Offline transaction signing: Unknown method parameter type: size_t (selsta)
- **#2656[^56]** Settings > Wallet: missing "Lock wallet" function (rating89us)
- **#2624[^57]** Scan of wallet export qr code using an iPhone camera app dials the phone number 147000 automatically. (satoshi-n)
- **#2722[^58]** Account: missing XMR suffix in balances (rating89us)
- **#2753[^59]** Submit each Monero build to VirusTotal as early as possible (mcgroarty)
- **#3034[^60]** *BSD build instructions? (dchmelik)
- **#3377[^61]** build: File name too long (sgulls)
- **#3857[^62]** [Feature] Lock Wallet & Bind it with Ctrl + L (elibroftw)
- **#3842[^63]** When Adding/Editing Remote Node, Pressing Enter in an Input Field Does Not Bind to Ok (elibroftw)
- **#3866[^64]** adding entry to address book edits description of another entry (Arimfexendrapus)



That's it for this week's dev activity report. I will try and publish one every Sunday. Let me know if I missed anything or if you want to see any other statistics/repos included in future reports. Feedback/edits: @ [/about](/about).

Previous reports are listed in the [[dev]](/tag/dev) section. 

**-3RA**

---

[^1]: https://github.com/monero-project/monero/pull/8220
[^2]: https://github.com/monero-project/monero/pull/8222
[^3]: https://github.com/monero-project/monero/pull/8223

[^4]: https://github.com/monero-project/monero-gui/pull/3868
[^5]: https://github.com/monero-project/monero-gui/pull/3869

[^6]: https://github.com/monero-project/monero-gui/pull/3862
[^7]: https://github.com/monero-project/monero-gui/pull/3863

[^8]: https://github.com/monero-project/monero/pull/8154
[^9]: https://github.com/monero-project/monero/pull/8158
[^10]: https://github.com/monero-project/monero/pull/8159
[^11]: https://github.com/monero-project/monero/pull/8169
[^12]: https://github.com/monero-project/monero/pull/8170
[^13]: https://github.com/monero-project/monero/pull/8186
[^14]: https://github.com/monero-project/monero/pull/8187
[^15]: https://github.com/monero-project/monero/pull/8190
[^16]: https://github.com/monero-project/monero/pull/8216
[^17]: https://github.com/monero-project/monero/pull/7675

[^18]: https://github.com/monero-project/monero-gui/pull/3470
[^19]: https://github.com/monero-project/monero-gui/pull/3719
[^20]: https://github.com/monero-project/monero-gui/pull/3720
[^21]: https://github.com/monero-project/monero-gui/pull/3851
[^22]: https://github.com/monero-project/monero-gui/pull/8209
[^23]: https://github.com/monero-project/monero-gui/pull/3860
[^24]: https://github.com/monero-project/monero-gui/pull/3862
[^25]: https://github.com/monero-project/monero-gui/pull/3865

[^26]: https://github.com/monero-project/monero-gui/issues/3864
[^27]: https://github.com/monero-project/monero-gui/issues/3867

[^28]: https://github.com/monero-project/monero/issues/60
[^29]: https://github.com/monero-project/monero/issues/1520
[^30]: https://github.com/monero-project/monero/issues/2522
[^31]: https://github.com/monero-project/monero/issues/3330
[^32]: https://github.com/monero-project/monero/issues/3234
[^33]: https://github.com/monero-project/monero/issues/3572
[^34]: https://github.com/monero-project/monero/issues/3537
[^35]: https://github.com/monero-project/monero/issues/3425
[^36]: https://github.com/monero-project/monero/issues/3394
[^37]: https://github.com/monero-project/monero/issues/3415
[^38]: https://github.com/monero-project/monero/issues/3513
[^39]: https://github.com/monero-project/monero/issues/3409
[^40]: https://github.com/monero-project/monero/issues/3519
[^41]: https://github.com/monero-project/monero/issues/3845
[^42]: https://github.com/monero-project/monero/issues/4497
[^43]: https://github.com/monero-project/monero/issues/4462
[^44]: https://github.com/monero-project/monero/issues/3874
[^45]: https://github.com/monero-project/monero/issues/3949
[^46]: https://github.com/monero-project/monero/issues/4141
[^47]: https://github.com/monero-project/monero/issues/4039
[^48]: https://github.com/monero-project/monero/issues/5233
[^49]: https://github.com/monero-project/monero/issues/5644
[^50]: https://github.com/monero-project/monero/issues/6323
[^51]: https://github.com/monero-project/monero/issues/6391
[^52]: https://github.com/monero-project/monero/issues/7259
[^53]: https://github.com/monero-project/monero/issues/8221
[^54]: https://github.com/monero-project/monero/issues/8073

[^55]: https://github.com/monero-project/monero-gui/issues/3861
[^56]: https://github.com/monero-project/monero-gui/issues/2656
[^57]: https://github.com/monero-project/monero-gui/issues/2624
[^58]: https://github.com/monero-project/monero-gui/issues/2722
[^59]: https://github.com/monero-project/monero-gui/issues/2753
[^60]: https://github.com/monero-project/monero-gui/issues/3034
[^61]: https://github.com/monero-project/monero-gui/issues/3377
[^62]: https://github.com/monero-project/monero-gui/issues/3857
[^63]: https://github.com/monero-project/monero-gui/issues/3842
[^64]: https://github.com/monero-project/monero-gui/issues/3866
