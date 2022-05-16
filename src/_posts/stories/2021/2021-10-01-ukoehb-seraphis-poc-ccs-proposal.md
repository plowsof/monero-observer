---
layout: post
category: story
title: UkoeHB submits Seraphis PoC CCS proposal
description: Monero contributor UkoeHB has submitted a CCS proposal that aims to develop a Seraphis C++ proof-of-concept.
tags: CCS
last_modified_at: 23 February 2022
---

Monero contributor UkoeHB[^1] has submitted a CCS proposal[^2] that aims to develop a Seraphis C++ proof-of-concept[^3]:

> Hi all, after some encouragement I decided to request funding for my ongoing work on Seraphis. Specifically, funding for future work on the Seraphis C++ proof-of-concept that I have been developing since the second week of September.

> My goal is for this code to be 95% production-ready.

UkoeHB shares several potential benefits and costs when comparing Seraphis/Lelantus-Spark with Triptych and RingCT:

- (+) membership proof delegation 
- (+) multi-tier wallet permissions
- (-) more implementation effort
- (-) all old addresses would become unusable (private keys/seeds/wallets don't need to be replaced)

He suggests that the last con might actually be an opportunity to improve Monero:

> Replacing old addresses is an opportunity to deprecate 'normal addresses' in favor of 'subaddresses' only. A uniform address format would simplify UX and various implementation details.

If this gets funded, the following tasks will be prioritized:

- core multisig functionality in Seraphis composition proof
- mock-up of 4 different Seraphis variants
- mock-up of Lelantus-Spark (probably... it turns out coding complex cryptographic algorithms like 
- advanced signature schemes is a lot of work)
- unit tests for all of the above
- comprehensive performance testing of all tx protocol mock-ups

> Once performance tests are complete, I will take a break of 1-4 weeks to finish the Seraphis paper.

UkoeHB has previously contributed to Monero by co-authoring *Zero to Monero* (1st[^4] and 2nd[^5] edition) and submitting several MRL & Monero core issues and PR's[^6].

```
Total funding: 92.6 XMR (50 USD + 0.2 XMR Rate).

ETA: TBD (6 weeks @ 40hr/wk = 240hrs).
```

A previous MO report[^7] discussing *Seraphis/Lelantus-Spark vs Triptych* might be relevant to this proposal. 

There is a high probability that one of the above will be part of Monero in the future. Regardless of which one the community picks, there is little doubt that the amount of decoys will increase as the ring signatures decrease in size and become more efficient, thus ultimately making Monero better.

To share your feedback, ask questions and support this proposal, consult !256[^2].

---

**Update 21/11/1: the proposal was fully funded.**

**Update 22/2/23: proposal completed[^8].**

---

[^1]: https://github.com/UkoeHB
[^2]: [https://repo.getmonero.org/monero-project/ccs-proposals/-/merge_requests/256](https://repo.getmonero.org/monero-project/ccs-proposals/-/merge_requests/256){:target="_blank"}
[^3]: https://github.com/UkoeHB/Seraphis
[^4]: https://web.getmonero.org/library/Zero-to-Monero-1-0-0.pdf
[^5]: https://web.getmonero.org/library/Zero-to-Monero-2-0-0.pdf
[^6]: https://github.com/monero-project/research-lab/issues/created_by/UkoeHB, https://github.com/monero-project/monero/issues/created_by/UkoeHB, https://github.com/monero-project/monero/issues/created_by/UkoeHB
[^7]: [/monero-community-torn-between-seraphis-triptych](/monero-community-torn-between-seraphis-triptych)
[^8]: [/ukoehb-completes-seraphis-poc-ccs-milestones](/ukoehb-completes-seraphis-poc-ccs-milestones)
