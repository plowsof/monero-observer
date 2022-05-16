---
layout: post
category: story
title: "UkoeHB submits new CCS proposal to continue work on Seraphis wallet PoC"
description: "UkoeHB has submitted a new CCS proposal to continue working on the Seraphis wallet proof-of-concept."
tags: CCS
---

UkoeHB[^1] has submitted a second CCS proposal[^2] to continue working on the Seraphis[^3] wallet proof-of-concept:

> Hi all, I closed out my previous Seraphis Wallet PoC CCS after consuming all the hours. There are additional tasks I would like to work on.

```
Total funding: 128 XMR (50 USD + 0.2 XMR Rate).

ETA: TBD (16 weeks @ 20hr/wk = 320hrs).
```

### Tasks overview

- Add tx builder plumbing for discretized tx fees.
- Consider using 16-byte address indices (instead of 7), with 2-byte encoded address index MACs (instead of 1)
- Implement a robust 'input selection' solver that takes advantage of statically-determinable tx weights.
- Implement a maximally-efficient and generic enote-scanning workflow.
- Build a wallet proof-of-concept that demonstrates all the 'transaction engineering' capabilities and implementation modularity of Seraphis/Jamtis. 
- Test out using x25519 for enote ECDH instead of ed25519, which may speed up enote scanning by a non-trivial amount (>10%).
- Miscellaneous code cleanup.

To learn more about UkoeHB's work, consult my previous report[^4].

To share your feedback, ask questions and support this proposal, consult !314[^2].



---

[^1]: https://github.com/UkoeHB
[^2]: [https://repo.getmonero.org/monero-project/ccs-proposals/-/merge_requests/314](https://repo.getmonero.org/monero-project/ccs-proposals/-/merge_requests/314){:target="_blank"}
[^3]: https://github.com/UkoeHB/Seraphis
[^4]: [/ukoehb-seraphis-wallet-poc-ccs-proposal/](/ukoehb-seraphis-wallet-poc-ccs-proposal/)
