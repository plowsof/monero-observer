---
layout: post
category: story
title: "rbrunner7 calls for dedicated effort to establish a clear migration path ahead of Seraphis/Jamtis Monero hardfork"
description: "rbrunner7 is calling for dedicated community efforts to establish a clear migration path ahead of Seraphis/Jamtis Monero hardfork."
tags: [wallets, pinned]
image: 
---

rbrunner7[^1] is calling[^2] for dedicated community efforts to establish a clear migration path ahead of the Seraphis[^3]/Jamtis[^4] Monero hardfork:

> I propose to start a dedicated effort to prevent such a very unfortunate outcome by working out a clear and well-documented migration path for wallets towards Seraphis and Jamtis, and start this effort not with the hardfork already looming at the horizon mere months away, but right now.

Although the exact HF date is unknown, 2023-2024 might be a decent estimate.

### The issue

Monero wallets will require an expensive, technically challenging and time-consuming extensive code refactoring in order to be compatible with the Monero core software post-HF:

> How can we make it possible for wallet app authors to start early enough with adapting their code to be ready for the hardfork to Seraphis and Jamtis in time?

> If we are not careful here we might end up with a situation where on the day of the hardfork only the CLI wallet is fully functional, the GUI wallet is still on its way, and it's unclear when smartphone wallets like Monerujo and Cake Wallet will be functional again thanks to updates.

### Proposed solutions

- A. define a new flexible `wallet3` API, implemented as a *thin layer* above `wallet2`[^5]
- B. deprecate any direct *binary* interfaces and fully rely on *RPC*[^6]

rbrunner7 has invited the community to get involved in the project: 

> People are needed to work on it, preferably people with knowledge already about the architecture and structure of the Monero codebase, and ideally some experience in API design plus project management on top of it.

In order to reach *loose consensus*, Monero devs, wallet authors and the broader Monero ecosystem should join the discussions[^2].

---

[^1]: https://github.com/rbrunner7
[^2]: [https://github.com/monero-project/monero/issues/8157](https://github.com/monero-project/monero/issues/8157){:target="_blank"}{:rel="nofollow"}
[^3]: https://github.com/UkoeHB/Seraphis
[^4]: https://gist.github.com/tevador/50160d160d24cfc6c52ae02eb3d17024
[^5]: https://github.com/monero-project/monero/blob/master/src/wallet/wallet2.cpp
[^6]: https://github.com/monero-project/monero/blob/master/src/rpc/core_rpc_server_commands_defs.h
