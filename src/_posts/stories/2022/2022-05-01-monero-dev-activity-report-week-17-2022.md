---
layout: post
category: story
title: "Monero Dev Activity Report - Week 17 2022: 37 PRs, 25 Issues"
description: "This weekly report aims to provide a big picture view of Monero development activity, increase community support for existing devs and, hopefully, encourage new contributions."
tags: dev
image: 
date: 2022-05-01 20:00
---

This weekly report aims to provide a big picture view of Monero development activity, increase community support for existing devs and, hopefully, encourage new contributions.

## 1 - PRs (37, 13:11:13)

Opened (13)

`monero-project/monero`:

- **#8293[^1]** BP+ optimization save one inversion in prover, use sc_muladd (ph4r05)
- **#8295[^2]** EPEE: Assimilate math_helper.h and document time_helper.h (jeffro256)
- **#8296[^3]** Gitian: refresh the stale Monero dir via --setup switch (mj-xmr)
- **#8299[^4]** feat(trezor): add HF15 support, BP+ (ph4r05)
- **#8300[^5]** Change "Github" to "GitHub" (zer-far)
- **#8301[^6]** Doxygen: Hide anonymous namespaces from documentation (jeffro256)
- **#8302[^7]** Update copyright to 2022 for Hardfork files (mj-xmr)
- **#8304[^8]** More tests for view tags (SChernykh)

`monero-project/monero-gui`:

- **#3902[^9]** WizardCreateDevice1: set default restore height to 1 (selsta)
- **#3903[^10]** WizardCreateDevice1: add Ledger Nano S Plus (selsta)
- **#3904[^11]** Added Fungibility to introduction (MaxQiu0108)
- **#3905[^12]** js: minimize frameless window when clicking on taskbar icon (selsta)
- **#3906[^13]** main: add compile time option to disable updates (selsta)

Closed (11)

`monero-project/monero`: 

- **#8288[^14]** Fix capitalisation of "Github" (zer-far) 
- **#8289[^15]** Dev (samisbakedham) 
- **#8292[^16]** Gitian: refresh submodules before compiling (mj-xmr) 
- **#8294[^17]** Fix capitalisation of "Github" (zer-far) 
- **#8297[^18]** Update year to 2022 (AkritW) 

`monero-project/monero-gui`: 

- **#3899[^19]** Release v0.14.1 merge to v0.14 (MaxQiu0108) 
- **#3885[^20]** main: don't async close wallet (selsta) 
- **#3669[^21]** Transfer: remove unnecessary line (selsta) 
- **#3900[^22]** Minor checks and added website at front (MaxQiu0108) 
- **#3655[^23]** Windows.js: minimize frameless window when clicking on taskbar icon (rating89us) 
- **#2731[^24]** TitleBar: add lock wallet button (rating89us) 

Merged (13)

`monero-project/monero`: 

- **#8178[^25]** Bump ring size to 16 for v15 (j-berman) 
- **#8248[^26]** Remove serialization/enableable (jeffro256) 
- **#8249[^27]** Remove /include (jeffro256) 
- **#8276[^28]** add a sanity check to RPC input data size (moneromooo-monero) 
- **#8273[^29]** build: prepare v0.17.3.2 (selsta) 
- **#8275[^30]** add a sanity check to RPC input data size (moneromooo-monero) 
- **#8260[^31]** Tiny: add .vscode/ to .gitignore (mj-xmr) 

`monero-project/monero-gui`:

- **#3887[^32]** workflows: action-docker-layer-caching v0.0.11 (selsta) 
- **#3888[^33]** FutureScheduler: delete unused function declarations (selsta) 
- **#3889[^34]** Mining: only update mining status when page is open (selsta) 
- **#3890[^35]** main: only update fiat price with open wallet (selsta) 
- **#3894[^36]** build: prepare v0.17.3.2 (selsta) 
- **#3897[^37]** TxConfirmationDialog: warn high fees (selsta) 

## 2 - ISSUES (25, 7:18)

Opened (7)

`monero-project/monero`: 

- **#8290[^38]** Unexpected error: Trezor returned failure: code=99, message=Firmware error (michnovka)
- **#8298[^39]** commission 19.73 xmr SOS (xmrmfjj2)

`monero-project/monero-gui`: 

- **#3893[^40]** GUI sometimes starts with smaller window (elibroftw)
- **#3895[^41]** [FR] Address Book contacts click to send (elibroftw)
- **#3896[^42]** [Performance BUG] Address book send transaction is slow (3s) (elibroftw)
- **#3898[^43]** High Fee Mitigation: Trusted Nodes for Simple Mode (reemuru)
- **#3907[^44]** "Export all History" CSV: output should be sorted by date (molecular)

Closed (18)

`monero-project/monero`:

- **#8268[^45]** busy wait (BebeSparkelSparkel)
- **#8286[^46]** Apple Silicon official binaries. (web-sharp)
- **#8291[^47]** M1 binaries (web-sharp)
- **#8168[^48]** Don't require --rpc-login with --rpc-access-control-origins (woodser)
- **#8305[^49]** 17.2 Debian patch (web-sharp)
- **#8306[^50]** Need Debian linux bare metal build (web-sharp)
- **#8303[^51]** 17.3.0 Rollback (web-sharp)

`monero-project/monero-gui`: 

- **#3840[^52]** Closing GUI After Wallet Open for a While Results in Infinite Loading Animation (elibroftw)
- **#3632[^53]** Crash of moned fixing pruned blockchain (Liger0)
- **#3355[^54]** Cannot start local Monerod on Ubuntu 20 (vanthome)
- **#3338[^55]** corrupted text everywhere (mikelpr)
- **#3805[^56]** Error: Couldn't connect to daemon (mochipancakes)
- **#3725[^57]** Cant create wallet on Ledger S with Monero GUI (FreeRide23)
- **#3722[^58]** Monero GUI crashing on Mac (b3K1ndRw1nd)
- **#3892[^59]** Monero Gui not showing funds (DarkAngel85)
- **#3845[^60]** Monero 'Oxygen Orion' (v0.17.3.0-release) Error: Couldn't connect to daemon: 127.0.0.1:18081 (ThomasAn73 )
- **#3901[^61]** [Question] How to upgrade to Monero GUI 17.3.2? (MaxQiu0108)
- **#3877[^62]** Ledger Nano S Plus support (AdamSiddique)

That's it for this week's dev activity report. I will try and publish one every Sunday. Let me know if I missed anything or if you want to see any other statistics/repos included in future reports. Feedback/edits: @ [/about](/about).

Previous reports are listed in the [[dev]](/tag/dev) section. 

**-3RA**

---

[^1]: https://github.com/monero-project/monero/pull/8293
[^2]: https://github.com/monero-project/monero/pull/8295
[^3]: https://github.com/monero-project/monero/pull/8296
[^4]: https://github.com/monero-project/monero/pull/8299
[^5]: https://github.com/monero-project/monero/pull/8300
[^6]: https://github.com/monero-project/monero/pull/8301
[^7]: https://github.com/monero-project/monero/pull/8302
[^8]: https://github.com/monero-project/monero/pull/8304

[^9]: https://github.com/monero-project/monero-gui/pull/3902
[^10]: https://github.com/monero-project/monero-gui/pull/3903
[^11]: https://github.com/monero-project/monero-gui/pull/3904
[^12]: https://github.com/monero-project/monero-gui/pull/3905
[^13]: https://github.com/monero-project/monero-gui/pull/3906

[^14]: https://github.com/monero-project/monero/pull/8288
[^15]: https://github.com/monero-project/monero/pull/8289
[^16]: https://github.com/monero-project/monero/pull/8292
[^17]: https://github.com/monero-project/monero/pull/8294
[^18]: https://github.com/monero-project/monero/pull/8297

[^19]: https://github.com/monero-project/monero-gui/pull/3899
[^20]: https://github.com/monero-project/monero-gui/pull/3885
[^21]: https://github.com/monero-project/monero-gui/pull/3669
[^22]: https://github.com/monero-project/monero-gui/pull/3900
[^23]: https://github.com/monero-project/monero-gui/pull/3655
[^24]: https://github.com/monero-project/monero-gui/pull/2731

[^25]: https://github.com/monero-project/monero/pull/8178
[^26]: https://github.com/monero-project/monero/pull/8248
[^27]: https://github.com/monero-project/monero/pull/8249
[^28]: https://github.com/monero-project/monero/pull/8276
[^29]: https://github.com/monero-project/monero/pull/8273
[^30]: https://github.com/monero-project/monero/pull/8275
[^31]: https://github.com/monero-project/monero/pull/8260

[^32]: https://github.com/monero-project/monero-gui/issues/3887
[^33]: https://github.com/monero-project/monero-gui/issues/3888
[^34]: https://github.com/monero-project/monero-gui/issues/3889
[^35]: https://github.com/monero-project/monero-gui/issues/3890
[^36]: https://github.com/monero-project/monero-gui/issues/3894
[^37]: https://github.com/monero-project/monero-gui/issues/3897

[^38]: https://github.com/monero-project/monero/issues/8290
[^39]: https://github.com/monero-project/monero/issues/8298

[^40]: https://github.com/monero-project/monero-gui/issues/3893
[^41]: https://github.com/monero-project/monero-gui/issues/3895
[^42]: https://github.com/monero-project/monero-gui/issues/3896
[^43]: https://github.com/monero-project/monero-gui/issues/3898
[^44]: https://github.com/monero-project/monero-gui/issues/3907

[^45]: https://github.com/monero-project/monero/issues/8268
[^46]: https://github.com/monero-project/monero/issues/8286
[^47]: https://github.com/monero-project/monero/issues/8291
[^48]: https://github.com/monero-project/monero/issues/8168
[^49]: https://github.com/monero-project/monero/issues/8305
[^50]: https://github.com/monero-project/monero/issues/8306
[^51]: https://github.com/monero-project/monero/issues/8303

[^52]: https://github.com/monero-project/monero-gui/issues/3840
[^53]: https://github.com/monero-project/monero-gui/issues/3632
[^54]: https://github.com/monero-project/monero-gui/issues/3355
[^55]: https://github.com/monero-project/monero-gui/issues/3338
[^56]: https://github.com/monero-project/monero-gui/issues/3805
[^57]: https://github.com/monero-project/monero-gui/issues/3725
[^58]: https://github.com/monero-project/monero-gui/issues/3722
[^59]: https://github.com/monero-project/monero-gui/issues/3892
[^60]: https://github.com/monero-project/monero-gui/issues/3845
[^61]: https://github.com/monero-project/monero-gui/issues/3901
[^62]: https://github.com/monero-project/monero-gui/issues/3877

