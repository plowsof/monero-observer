---
layout: post
category: story
title: "MRL's UkoeHB submits Seraphis wallet PoC CCS proposal"
description: "MRL's UkoeHB has submitted a CCS proposal that aims to build a Seraphis wallet proof-of-concept."
tags: CCS
last_modified_at: 2022-03-26
---

MRL[^0]'s UkoeHB[^1] has submitted a new CCS proposal[^2] that aims to build a Seraphis[^3] wallet proof-of-concept:

> These tasks will be implemented in my seraphis_lib branch. [..] Build a wallet proof-of-concept that demonstrates all the 'transaction engineering' capabilities and implementation modularity of Seraphis/Jamtis. 

```
Total funding: 81.4 XMR (50 USD + 0.2 XMR Rate).

ETA: TBD (8 weeks @ 20hr/wk = 160hrs).
```

### Tasks overview

- build a [Seraphis] wallet proof-of-concept 
- test out using x25519 for enote ECDH instead of ed25519, which may speed up enote scanning by a non-trivial amount (>10%)
- add validation code and plumbing for tx_extra fields
- add tx builder plumbing for tx fees
- add multisig tx builders for Seraphis (with unit tests) after the master branch is updated with PR #7877
- miscellaneous code cleanup

UkoeHB has previously contributed to Monero by co-authoring *Zero to Monero* (1st[^4] and 2nd[^5] edition) and submitting several MRL & Monero core issues and PR's[^6]. To learn more, consult the dev's previous CCS proposal[^7].

To share your feedback, ask questions and support this proposal, consult !290[^2].


---

**Update 22/3/14: moved to funding[^8].**

**Update 22/3/26: fully funded[^9].**

---

[^0]: https://github.com/monero-project/research-lab
[^1]: https://github.com/UkoeHB
[^2]: [https://repo.getmonero.org/monero-project/ccs-proposals/-/merge_requests/290](https://repo.getmonero.org/monero-project/ccs-proposals/-/merge_requests/290){:target="_blank"}
[^3]: https://github.com/UkoeHB/Seraphis
[^4]: https://web.getmonero.org/library/Zero-to-Monero-1-0-0.pdf
[^5]: https://web.getmonero.org/library/Zero-to-Monero-2-0-0.pdf
[^6]: https://github.com/monero-project/research-lab/issues/created_by/UkoeHB, https://github.com/monero-project/monero/issues/created_by/UkoeHB
[^7]: https://repo.getmonero.org/monero-project/ccs-proposals/-/merge_requests/256
[^8]: [/ukoehb-seraphis-wallet-poc-ccs-proposal-ready-funding/](/ukoehb-seraphis-wallet-poc-ccs-proposal-ready-funding/)
[^9]: [/ukoehb-ccs-proposal-seraphis-wallet-poc-ccs-proposal-fully-funded/](/ukoehb-ccs-proposal-seraphis-wallet-poc-ccs-proposal-fully-funded/)
