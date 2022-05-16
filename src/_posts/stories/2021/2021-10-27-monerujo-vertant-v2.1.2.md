---
layout: post
category: story
title: Monerujo v2.1.2 Vertant release fixes sideshifting bug
description: The newest version of Monerujo, v2.1.2 Vertant has been released and it upgrades to the latest Monero core version which fixes the decoy selection bug.
tags: wallets
image: 
---

The newest Monerujo[^1] release, v2.1.2 *Vertant*[^2] is out. 

This point release fixes the `settleAmount must be greater than 0` bug when sideshifting.

Notes:

> Wallet files are stored in app-internal storage accessible only by the app on non-rooted devices. External storage is no longer used. Current wallets will be copied to app-internal storage once. After that, wallets can be imported as zip files containing the wallet files (<wallet>.keys & <wallet>).

> Warning: Uninstalling the app will delete your wallets on the device! Use the backup function to backup your wallets - you will need the CrAzYpass (aka "Restore Password") in order to open backed-up wallets - also in other apps.

Before usage, it is recommended to verify that you have downloaded the correct file using the SHA256 hashes listed in the repository[^2].

To support the open-source project, donate to the XMR addresses listed on Github or on the Monerujo Funding site[^3] if you wish to support a specific feature.

We can expect support for .onion nodes to come soon[^4], as the community has fully funded that project recently.
 
---

[^1]: https://monerujo.io
[^2]: [https://github.com/m2049r/xmrwallet/releases/tag/v2.1.2](https://github.com/m2049r/xmrwallet/releases/tag/v2.1.2){:target="_blank"}{:rel="nofollow"}, https://f-droid.monerujo.io/fdroid/repo/ (F-droid)
[^3]: https://funding.monerujo.app/
[^4]: https://nitter.net/monerujowallet/status/1452632681146093570#m
