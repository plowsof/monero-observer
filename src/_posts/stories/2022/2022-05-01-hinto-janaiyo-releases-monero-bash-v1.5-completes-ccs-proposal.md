---
layout: post
category: story
title: hinto-janaiyo completes CCS proposal with release of 'monero-bash' v1.5
description: "hinto-janaiyo has released 'monero-bash' v1.5, essentially finalizing all the milestones for the associated CCS proposal."
tags: [CCS, mining]
image: 
---

hinto-janaiyo[^1] has released *monero-bash*[^2] v1.5[^3], essentially finalizing all the milestones for the associated CCS proposal[^4]:

> All milestones finished including 3.5 XMR: RPC/Daemon API integration[^5]

## Changes

- Monerod JSON RPC interface
- `p2pool` displays latest share found & shares per day
- mini pool fix - reconfigure with `monero-bash config` or edit `p2pool.json`
- `p2pool.cache/p2pool_peers.txt` are kept between upgrades for faster sync

The sources, SHA256SUM and .asc files can be found on Github[^3]. Always verify before using.

To learn more about the project, read the associated CCS proposal[^4] and my previous report[^6].

---

[^1]: https://github.com/hinto-janaiyo
[^2]: https://github.com/hinto-janaiyo/monero-bash
[^3]: [https://github.com/hinto-janaiyo/monero-bash/releases/tag/v1.5](https://github.com/hinto-janaiyo/monero-bash/releases/tag/v1.5){:target="_blank"}
[^4]: https://ccs.getmonero.org/proposals/monero-bash.html
[^5]: https://repo.getmonero.org/monero-project/ccs-proposals/-/merge_requests/297#note_16129
[^6]: [/hinto-janaiyo-submits-ccs-proposal-monero-bash/](/hinto-janaiyo-submits-ccs-proposal-monero-bash/)
