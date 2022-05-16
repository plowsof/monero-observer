---
layout: post
category: story
title: "kopipe proposes $3,099 bounty for Monero vanity address generator that uses OpenCL or CUDA"
description: "kopipe has proposed a $3,099 bounty for the creation of a Monero vanity address generator CLI app that uses either OpenCL or CUDA and is at least 4 times faster than the CPU-driven 'vanity-monero' tool."
tags: bounties
image: 
date: 2022-04-17 20:00
last_modified_at: 2022-04-18
---

kopipe[^1] has proposed a $3,099 bounty[^2] for the creation of a Monero vanity address generator CLI app that uses either OpenCL or CUDA and is at least 4 times faster than the existing CPU-driven *vanity-monero*[^3] tool:

> Monero vanity address generation can currently only be done via CPU. [..] the Modular Font Editor K Foundation, Incorporated, a New Jersey non-profit [..] is offering a bounty of $3,099 to be paid however the accepting user prefers for a Monero (XMR) vanity address program meeting these specs [..]

### Specs

- works on GNU/Linux
- works with NVIDIA cards (minimum: NVIDIA GeForce RTX 3080 Laptop GPU)
- is command line driven
- uses either CUDA or OpenCL 
- accepts at least a single search prefix on the command line for the public receive key
- is at least 4x faster than https://github.com/monero-ecosystem/vanity-monero
- reports the number of keys it's considering every n seconds

Note that the bounty will **not** be paid unless the software is licensed under the Apache 2.0 license and includes this copyright line: 

`Support for this software's development was paid for by Fredrick R. Brennan's Modular Font Editor K Foundation, Inc.`

The bounty was also posted on Monero Bounties[^4], but it is unclear if the donation bot is fully operational again[^5].

To learn more about generating custom/vanity XMR addresses, consult the *vanity-monero* repository README[^6].

---

**Update: bounty paid to sech1[^7] for *vanity_xmr_cuda*[^8].**

---

[^1]: https://bitcointalk.org/index.php?action=profile;u=133423
[^2]: [https://bitcointalk.org/index.php?topic=5394915.msg59884817](https://bitcointalk.org/index.php?topic=5394915.msg59884817){:target="_blank"}
[^3]: https://github.com/monero-ecosystem/vanity-monero
[^4]: https://bounties.monero.social/posts/63/
[^5]: [/monero-bounties-bot-broken/](/monero-bounties-bot-broken/)
[^6]: https://github.com/monero-ecosystem/vanity-monero#readme
[^7]: https://bitcointalk.org/index.php?topic=5394915.msg59900519#msg59900519
[^8]: https://github.com/SChernykh/vanity_xmr_cuda
