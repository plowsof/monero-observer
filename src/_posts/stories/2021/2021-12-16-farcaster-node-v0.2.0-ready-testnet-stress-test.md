---
layout: post
category: story
title: Farcaster Node v0.2.0 ready for first Testnet stress test
description: "The Farcaster Project has released v0.2.0 of the Farcaster Node with support for running parallel swaps."
tags: services
image: 
---

The Farcaster Project[^0] has released v0.2.0[^1] of the Farcaster Node[^2] with support for running parallel swaps:

> Working on this the past few months has been incredibly fun, challenging, educational and intense. The upcoming milestone 3 focuses on making what we built user friendly, thus the more people outside of our circle of devs test and provide feedback, the better! -**TheCharlatan**[^3]

The P2P XMR-BTC atomic swap software is ready for its first Testnet stress test.

> From preliminary testing, a lean server with 2 GB of RAM and 2 CPUs is enough for running at least 50 swaps in parallel.

### Changes

- Support running parallel swaps over different peer connections through different
ports

Tor support was not implemented in this early version and your IP address will be logged if you swap against any of the offers on farcaster.dev:

> Tor support solves that, but not yet functional :(

> Swaps against us will be logged, this data will be used for improving the software, debugging what went wrong, etc. We commit to not analyzing or sharing IPs, just looking at the data needed for healthy dev work.  

Note that the tech is still experimental. Do not try using the software on mainnet or with real money:

> Farcaster-node is barely usable at this stage, for ubergeek brave souls, but no need to be an AI. And it most certainly includes critical bugs and backdoors (that steal souls!) that we among others will use to exploit you! Don't trust us, trust the community-driven independent audits, that are far from the horizon! Till then, you're gambling. 

Read the announcement thread[^4] and visit the website[^5] for more information:

> AIs like experimenting with Humans. farcaster.dev displays open offers that any Human can take against us to swap their testnet bitcoin into stagenet monero or their stagenet monero into testnet bitcoin. 

You can view the list of devs working on Farcaster by visiting plowsof[^6]'s Monerodevs[^7] website.

The project was funded via the CCS system[^8] in September 2020. The Monero community has donated a total of 2727 XMR for this proposal.

To get involved with the project, join *#monero-swap* on IRC/Libera. To test the software, you could try taking Sethforprivacy[^9]'s offer[^10]'[^11].

---

[^0]: https://github.com/farcaster-project
[^1]: [https://github.com/farcaster-project/farcaster-node/releases/tag/v0.2.0](https://github.com/farcaster-project/farcaster-node/releases/tag/v0.2.0){:target="_blank"}{:rel="nofollow"}
[^2]: https://github.com/farcaster-project/farcaster-node
[^3]: https://github.com/TheCharlatan, https://libredd.it/r/Monero/comments/rhe6rg/farcaster_node_a_decentralized_p2p_atomic_swap/hoq24xv/
[^4]: [https://libredd.it/r/Monero/comments/rhe6rg/](https://libredd.it/r/Monero/comments/rhe6rg/){:target="_blank"}{:rel="nofollow"}
[^5]: https://farcaster.dev
[^6]: https://github.com/plowsof
[^7]: https://monerodevs.org/farcaster-atomic-swaps-btc-xmr.html
[^8]: https://ccs.getmonero.org/proposals/h4sh3d-atomic-swap-implementation.html
[^9]: https://nitter.pussthecat.org/sethforprivacy
[^10]: https://nitter.pussthecat.org/sethforprivacy/status/1471540353685729282#m
[^11]: https://paste.sethforprivacy.com/?70601748ab6558ea#2Q48Nt3GmFRrRWmDnnNvVGnfY7H7chsayVdpQNrF6WAN
