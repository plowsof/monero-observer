---
layout: post
category: story
title: "Monero Dev Activity Report - Week 16 2022: 31 PRs, 12 Issues"
description: "This weekly report aims to provide a big picture view of Monero development activity, increase community support for existing devs and, hopefully, encourage new contributions."
tags: dev
image: 
---

This weekly report aims to provide a big picture view of Monero development activity, increase community support for existing devs and, hopefully, encourage new contributions.

## 1 - PRs (31, 16:3:12)

Opened (16)

`monero-project/monero`:

- **#8264[^1]** Tests: libwallet_api_tests fixing scripts (mj-xmr)
- **#8266[^2]** depends: update unbound to 1.15.0 (selsta)
- **#8270[^3]** Update README.md: Add v15 network upgrade (garth-xmr)
- **#8273[^4]** build: prepare v0.17.3.2 (selsta)
- **#8275[^5]** add a sanity check to RPC input data size (moneromooo-monero)
- **#8276[^6]** add a sanity check to RPC input data size (moneromooo-monero)
- **#8277[^7]** Preserve commitment format inside transactions (kayabaNerve)
- **#8278[^8]** EPEE: Remove hmac-md5 (jeffro256)
- **#8279[^9]** EPEE: Remove gzip_encoding.h (jeffro256)
- **#8280[^10]** DOCS: Add documentation for EPEE Portable Storage (jeffro256)
- **#8281[^11]** readme: arch/fedora deps + small fixes (hinto-janaiyo)
- **#8285[^12]** wallet2: Erase payments for self-spends or change when importing key images (j-berman)

`monero-project/monero-gui`:

- **#3887[^13]** workflows: action-docker-layer-caching v0.0.11 (selsta)
- **#3888[^14]** FutureScheduler: delete unused function declarations (selsta)
- **#3889[^15]** Mining: only update mining status when page is open (selsta)
- **#3890[^16]** main: only update fiat price with open wallet (selsta)

Closed (3)

`monero-project/monero`: 

- **#8271[^17]** Monero project master (samisbakedham) 
- **#8272[^18]** Replace in-house MD5 with OpenSSL (jeffro256) 
- **#8287[^19]** Fix capitalisation of "Github" (zer-far) 

`monero-project/monero-gui`: none

Merged (12)

`monero-project/monero`: 

- **#8232[^20]** Added support for Ledger Nano S Plus (hbs) 
- **#8239[^21]** Added support for Ledger Nano S Plus [release-v0.17] (selsta) 
- **#8240[^22]** randomx: update submodule (selsta) 
- **#8241[^23]** randomx: update submodule [release-v0.17] (selsta) 
- **#8245[^24]** simplewallet: fix integrated_address output string (selsta) 
- **#8246[^25]** Makefile: fix spelling of CMAKE_BUILD_TYPE value (selsta) 
- **#8247[^26]** readme: small fixes (hinto-janaiyo) 
- **#8254[^27]** wallet2: use BP+ for cold signing (moneromooo-monero) 

`monero-project/monero-gui`:

- **#3869[^28]** TitleBar: Remove lock icon on essentials display (reemuru) 
- **#3871[^29]** Docker: update Qt 5.15.2 -> 5.15.3 (selsta) 
- **#3875[^30]** Docker: Update zlib for android (devhyper) 
- **#3879[^31]** cmake: bump windows deploy lib versions, update workflows (selsta) 

## 2 - ISSUES (12, 5:7)

Opened (5)

`monero-project/monero`: 

- **#8268[^32]** busy wait (BebeSparkelSparkel)
- **#8274[^33]** eternal loading wallet...(rpc) (dmitrykrylov18)
- **#8286[^34]** Apple Silicon official binaries. (web-sharp)

`monero-project/monero-gui`: 

- **#3891[^35]** The installed GUI wallet cannot find wallets in C:\Users\%USER%\Documents\Monero\wallets (elibroftw)
- **#3892[^36]** Monero Gui not showing funds (DarkAngel85)

Closed (7)

`monero-project/monero`:

- **#8265[^37]** Locate wallet file (arkadiy-telegin)
- **#8267[^38]** How many addresses are allowed to be transferred at one time? (EWIT521)
- **#8269[^39]** Why not add utility tokens on Monero, it will be useful for stablecoins! (iafi01)
- **#8282[^40]** What to do when preparing for Monero hardfork. (MaxQiu0108)
- **#8283[^41]** Monerod blocked by MSE (MaxQiu0108)
- **#8284[^42]** What to prepare for next hardfork (MaxQiu0108)

`monero-project/monero-gui`: 

- **#3714[^43]** Plans to integrate P2Pool at some point? (Pax2513)

That's it for this week's dev activity report. I will try and publish one every Sunday. Let me know if I missed anything or if you want to see any other statistics/repos included in future reports. Feedback/edits: @ [/about](/about).

Previous reports are listed in the [[dev]](/tag/dev) section. 

**-3RA**

---

[^1]: https://github.com/monero-project/monero/pull/8264
[^2]: https://github.com/monero-project/monero/pull/8266
[^3]: https://github.com/monero-project/monero/pull/8270
[^4]: https://github.com/monero-project/monero/pull/8273
[^5]: https://github.com/monero-project/monero/pull/8275
[^6]: https://github.com/monero-project/monero/pull/8276
[^7]: https://github.com/monero-project/monero/pull/8277
[^8]: https://github.com/monero-project/monero/pull/8278
[^9]: https://github.com/monero-project/monero/pull/8279
[^10]: https://github.com/monero-project/monero/pull/8280
[^11]: https://github.com/monero-project/monero/pull/8281
[^12]: https://github.com/monero-project/monero/pull/8285

[^13]: https://github.com/monero-project/monero-gui/pull/3887
[^14]: https://github.com/monero-project/monero-gui/pull/3888
[^15]: https://github.com/monero-project/monero-gui/pull/3889
[^16]: https://github.com/monero-project/monero-gui/pull/3890

[^17]: https://github.com/monero-project/monero/pull/8271
[^18]: https://github.com/monero-project/monero/pull/8272
[^19]: https://github.com/monero-project/monero/pull/8287

[^20]: https://github.com/monero-project/monero/pull/8232
[^21]: https://github.com/monero-project/monero/pull/8239
[^22]: https://github.com/monero-project/monero/pull/8240
[^23]: https://github.com/monero-project/monero/pull/8241
[^24]: https://github.com/monero-project/monero/pull/8245
[^25]: https://github.com/monero-project/monero/pull/8246
[^26]: https://github.com/monero-project/monero/pull/8247
[^27]: https://github.com/monero-project/monero/pull/8254

[^28]: https://github.com/monero-project/monero-gui/pull/3869
[^29]: https://github.com/monero-project/monero-gui/pull/3871
[^30]: https://github.com/monero-project/monero-gui/pull/3875
[^31]: https://github.com/monero-project/monero-gui/pull/3879

[^32]: https://github.com/monero-project/monero/issues/8268
[^33]: https://github.com/monero-project/monero/issues/8274
[^34]: https://github.com/monero-project/monero/issues/8286

[^35]: https://github.com/monero-project/monero-gui/issues/3891
[^36]: https://github.com/monero-project/monero-gui/issues/3892

[^37]: https://github.com/monero-project/monero/issues/8265
[^38]: https://github.com/monero-project/monero/issues/8267
[^39]: https://github.com/monero-project/monero/issues/8269
[^40]: https://github.com/monero-project/monero/issues/8282
[^41]: https://github.com/monero-project/monero/issues/8283
[^42]: https://github.com/monero-project/monero/issues/8284

[^43]: https://github.com/monero-project/monero-gui/issues/3714

