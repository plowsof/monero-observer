---
layout: post
category: story
title: COMIT releases v0.9.0 of their XMR-BTC atomic swap implemenation
description: COMIT has released version 0.9.0 of their XMR-BTC atomic swap tool, which includes two bug fixes.
tags: services
image: 
---

COMIT[^1] has released version 0.9.0[^2] of their XMR-BTC atomic swap tool[^3].

This update brings several changes and additions to the code, including:

- Timestamping is now enabled by default even when the ASB is not run inside an interactive terminal.

- The `cancel`, `refund` and `punish` subcommands in ASB and CLI are run with the `--force` by default and the `--force` option has been removed.

- ASB and CLI can migrate their data to sqlite to store swaps and related data.

- Added a `disable-timestamp` flag to the ASB that disables timestamps from logs.

- Removed the `bitcoin-target-block` argument from the `balance` subcommand on the CLI.

Other modifications and a database migration guide can be found in the Github repository[^2].


---

[^1]: https://comit.network
[^2]: [https://github.com/comit-network/xmr-btc-swap/releases/tag/0.9.0](https://github.com/comit-network/xmr-btc-swap/releases/tag/0.9.0){:target="_blank"}{:rel="nofollow"}
[^3]: https://github.com/comit-network/xmr-btc-swap
