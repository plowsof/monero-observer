---
layout: post
category: story
title: UkoeHB invites Monero community to discuss potential Seraphis address schemes
description: "Monero contributor UkoeHB has invited the community to discuss potential address schemes for the upcoming Seraphis implementation."
tags: [dev, pinned]
image: 
date: 2021-11-12 22:30
---

Monero contributor UkoeHB[^1] has invited the community to discuss[^2] potential address schemes for the upcoming Seraphis[^3] implementation:

> Seraphis is not compatible with CryptoNote addressing, due to a different key image design compared to CryptoNote. However, it is compatible with a variety of interesting addressing schemes. In this issue I'd like to present those schemes, so discussion can have a point of reference.

It is worth noting that when this is implemented, all users will have to generate new public addresses from their private keys: 

- old public addresses would become unusable
- old wallets would still be usable

For more information, read Koe's CCS proposal[^3]'[^4] to develop a Seraphis C++ proof-of-concept.

---

[^1]: https://github.com/UkoeHB
[^2]: [https://github.com/monero-project/research-lab/issues/92](https://github.com/monero-project/research-lab/issues/92){:target="_blank"}{:rel="nofollow"}
[^3]: [/ukoehb-seraphis-poc-ccs-proposal/](/ukoehb-seraphis-poc-ccs-proposal/)
[^4]: https://repo.getmonero.org/monero-project/ccs-proposals/-/merge_requests/256
