---
layout: post
category: story
title: "akimayumi forks Monerujo into 'Shruum' alpha wallet"
description: "akimayumi has forked Monerujo, the Android Monero wallet, into 'Shruum', an alpha state Monero-only wallet with mandatory Tor usage and planned I2P support."
tags: wallets
image: 
date: 2022-04-16 20:00
last_modified_at: 2022-04-19
---

akimayumi[^1] has forked Monerujo[^2], the Android Monero wallet, into *Shruum*[^3], an alpha state Monero-only wallet with *mandatory Tor usage* and planned I2P support:

> I am currently working on a fork of Monerujo that makes Tor mandatory, and features a "Monero-only" design in order to maintain privacy and anonymity. Because of the mandatory Tor usage, the altcoin payment system within the app that was powered by SideShift has been removed, as SideShift now blocks Tor users.[^4]

## Changes

- mandatory Tor usage[^5]
- removed fiat conversion and SideShift integration (SideShift blocks Tor users)[^6]'[^7]
- removed translations[^8]
- some theme changes and other small fixes[^9]
- mandatory passwords for wallets
- fiat rates and rate fetching are gone for a "Monero-only" experience, and to limit network calls
- NFC support has been removed
- Ledger Nano S Plus support
- other UI and theme changes


Currently the app can only be compiled manually. Stagenet .APKs can be downloaded from akimayumi's website[^10].

---

**Update: add to the list of changes.**

---

[^1]: https://git.mayumi.one/mayumi
[^2]: https://github.com/m2049r/xmrwallet
[^3]: [https://git.mayumi.one/mayumi/shruum](https://git.mayumi.one/mayumi/shruum){:target="_blank"}
[^4]: https://libredd.it/u4hruf/
[^5]: https://git.mayumi.one/mayumi/shruum/commit/5c93131158a91e0f753b9b34b22201ff3ab38a72
[^6]: https://git.mayumi.one/mayumi/shruum/commit/9638c27aa35e1dd85e41f543810409c1af84d04b
[^7]: https://git.mayumi.one/mayumi/shruum/commit/8d05ccaea29f5168a4a4981141322008a46cb9db
[^8]: https://git.mayumi.one/mayumi/shruum/commit/4f9c7877ce64f636be287c165fd96b60561da66b
[^9]: https://git.mayumi.one/mayumi/shruum/commits/branch/master
[^10]: [https://mayumi.one/](https://mayumi.one/){:target="_blank"}
