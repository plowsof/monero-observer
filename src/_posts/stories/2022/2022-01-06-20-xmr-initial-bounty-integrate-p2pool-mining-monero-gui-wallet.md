---
layout: post
category: story
title: "20 XMR initial bounty for integration of P2Pool mining into Monero GUI wallet"
description: "xmrvsbeast has proposed a bounty for the integration of P2Pool mining into Monero GUI wallet."
tags: bounties
image: 
---

xmrvsbeast[^1] has proposed a bounty[^2] for the integration of P2Pool mining into Monero GUI wallet:

> Enable users to mine on p2pool right from the GUI wallet with one click.

```
Total Bounty: 20 XMR (to date)
```

### Requirements

- Code is open-source
- Code is submitted to the Monero repo as a pull-request 
- Pull request properly and functionally integrates p2pool into GUI wallet w/o need for any extra downloads
- Include feature to input optional p2pool command line parameters such as --host
- Auto select appropriate side-chain (main or mini) or default to mini if not possible
- Pull request is accepted into Monero's code base after review

One important thing to note is that the bounty can only be claimed if the Monero GUI Wallet maintainers actually accept the PR, as Rucknium[^3] pointed out:

> What if the Monero GUI Wallet maintainers decide they don't want p2pool functionality in the main codebase?

> An alternative would be to accept the bounty as being completed if the pull request is submitted, but not necessarily accepted. Then a fork of the wallet with p2pool could be maintained.

To start working on the project yourself, you should make your intentions public by posting a comment in the bounty's thread.

To increase the bounty you can contribute some XMR to the bounty address posted by the *Monero Bounties Bot*[^2].

---

[^1]: https://libredd.it/r/xmrvsbeast
[^2]: [https://bounties.monero.social/posts/53](https://bounties.monero.social/posts/53){:target="_blank"}
[^3]: https://github.com/Rucknium
