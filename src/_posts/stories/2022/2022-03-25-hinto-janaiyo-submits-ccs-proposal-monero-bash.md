---
layout: post
category: story
title: "hinto-janaiyo submits CCS proposal to build	monero-bash wrapper for Linux"
description: "hinto-janaiyo has submitted a CCS proposal looking to further develop 'monero-bash', a Monero wrapper, written in Bash, for Linux."
tags: CCS
date: 2022-03-25 20:00
last_modified_at: 2022-04-11
---

hinto-janaiyo[^1] has submitted a CCS proposal[^2] looking to further develop *monero-bash*[^3], a Monero wrapper, written in Bash, for Linux:

> monero-bash does what bash normally does: it glues together multiple programs in a more automatic fashion [..]: monerod, monero-wallet-cli, monero-rpc, (p2pool planned...)

```
Total funding: 10 XMR.

ETA: TBD.
```

> monero-bash abstracts monero-cli commands into interactive prompts and linux-like syntax

The extra layer might be of use to anyone that wants to automatically set up and run all of the tools (wallet, node, miner) on any number of machines and benefit from a central software that manages everything.

### Features (implemented)

- Automatic monero release upgrades, verified with SHA256SUMS
- Software and wallet management
- Easy wallet/daemon control
- Price stats from API

### Milestones

- M1: Integrated P2Pool Mining (5 XMR)
- M2: RPC/Daemon API integration (3.5 XMR)
- M3: Mining quickstart commands (1 XMR)
- M4: Automated encrypted wallet backup (0.25 XMR)
- M5: Auto GPG key verification for binaries (0.25 XMR)

To learn more about the script, its folder structure and configuration, consult the monero-bash guide[^4].

hinto-janaiyo is also maintaining XMRig-Auto-Build[^5] and monero-toolchain[^6].

To read the full proposal, share your feedback, ask questions and support this CCS, consult !297[^2].

---

**Update 22/4/4: moved to funding[^7].**

**Update 22/4/11: M2 canceled[^8].**

---

[^1]: https://github.com/hinto-janaiyo
[^2]: [https://repo.getmonero.org/monero-project/ccs-proposals/-/merge_requests/297](https://repo.getmonero.org/monero-project/ccs-proposals/-/merge_requests/297){:target="_blank"}
[^3]: https://github.com/hinto-janaiyo/monero-bash
[^4]: https://github.com/hinto-janaiyo/monero-bash/blob/main/docs/help.md
[^5]: [/hinto-janaiyo-releases-xmrig-auto-build-v1.2/](/hinto-janaiyo-releases-xmrig-auto-build-v1.2/)
[^6]: [/hinto-janaiyo-releases-monero-toolchain-v2.0.0/](/hinto-janaiyo-releases-monero-toolchain-v2.0.0/)
[^7]: [/hinto-janaiyo-monero-bash-ccs-proposal-ready-funding](/hinto-janaiyo-monero-bash-ccs-proposal-ready-funding)
[^8]: https://repo.getmonero.org/monero-project/ccs-proposals/-/merge_requests/297#note_15833
