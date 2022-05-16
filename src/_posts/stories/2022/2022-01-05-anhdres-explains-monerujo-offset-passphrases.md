---
layout: post
category: story
title: Andres explains recently introduced Monerujo offset passphrases
description: "Andres has written an article in which he explains how the recently introduced offset passphrases work in Monerujo."
tags: wallets
date: 2022-01-05 21:00
---

Andres[^1] has written an article[^2] in which he explains how the recently introduced offset passphrases work in Monerujo[^3]:

> Since version 2.3.1 Monerujo comes with a feature called CryptSeed™ that allows you to create and restore a wallet that has a very special, yet very normal-looking seed.

Monerujo users can opt to add an extra (26th) word to their wallet's seed. 

The custom passphrase shifts the original seed in a reproductible way, which gives a different seed, but the same different seed every time.

This provides an extra layer of security, as one could write down the original seed in one place, and store the offset passphrase in another. Whoever finds the seed will only get access to the *decoy* wallet, which should be empty, and cannot steal the moneroj stored in the *real* wallet.

13 contributors have donated a total of 3 XMR to fund this project on the Monerujo Funding[^4] page:

> Support for Monero seeds with an extra passphrase for improved security

The feature was shipped with Monerujo v2.3.1 *Doménikos*, which was realeased a few days ago[^5].

---

[^1]: https://nitter.net/anhdres, https://anhdr.es/
[^2]: [https://anhdres.medium.com/how-a-mnemonic-seed-with-offset-passphrase-works-in-monerujo-416ff5198b2e](https://anhdres.medium.com/how-a-mnemonic-seed-with-offset-passphrase-works-in-monerujo-416ff5198b2e){:target="_blank"}{:rel="nofollow"}
[^3]: https://www.monerujo.io/
[^4]: https://funding.monerujo.app/
[^5]: [/monerujo-domenikos-v2.3.1-released-seed-encryption-support/](/monerujo-domenikos-v2.3.1-released-seed-encryption-support/)
