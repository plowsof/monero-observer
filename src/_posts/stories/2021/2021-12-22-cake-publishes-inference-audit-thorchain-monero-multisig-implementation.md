---
layout: post
category: story
title: "Cake Wallet publishes Inference's audit of Thorchain's Monero multisig implementation"
description: "Cake Wallet has published Inference's audit of Thorchain's Monero multisig implementation."
tags: [security, services]
---

Cake Wallet[^1] has published Inference[^2]'s audit[^3] of Thorchain[^4]'s Monero multisig implementation[^5]:

> A few weeks ago, Cake Wallet reached out to auditors to review Thorchain's Monero multisig implementation. This is a critical part of Thorchain's code, since it is expected to be used to store native XMR used for liquidity providing and other functions of the Thorchain network.

The audit uncovered 2 potential security issues with low impact:

```
- S-CKW-001: [sign_multisig_parallel()] Unchecked parsing result (Exploitability: medium / Impact: low)
- S-CKW-002: [accu_multisig()] Undefined Behavior with Empty Signatures (Exploitability: low / Impact: low)
```

The report also produced 5 observations related to defense-in-depth, reliability, and performance:

```
- O-CKW-01: [Dockerfile] Leaked IP address
- O-CKW-02: [Dockerfile] unused ports
- O-CKW-03: Unused variables
- O-CKW-04: [RPC] on_check_transaction() can fail if two destinations have
the same amount
- O-CKW-05: [RPC] on_check_transaction() inconsistent failure handling
```

Before Thorchain can use Monero multisig, some PRs[^6] still have to be reviewed and merged. That would fix the recently disclosed vulnerabilities in the implementation of Monero multisignature wallets code, as previously reported[^7]. 

More details about this development can be found in Cake's announcement thread[^8].

---

[^1]: https://cakewallet.com
[^2]: https://inference.ag/
[^3]: [https://cakewallet.com/assets/docs/2021-12-20-cakewallet-thorchain-audit.pdf](https://cakewallet.com/assets/docs/2021-12-20-cakewallet-thorchain-audit.pdf){:target="_blank"} (PDF)
[^4]: https://thorchain.org/
[^5]: https://gitlab.com/thorchain/tss/monero-sign/
[^6]: https://github.com/monero-project/monero/pull/8113, https://github.com/monero-project/monero/pull/8114
[^7]: [/vulnerabilities-identified-monero-multisignature-wallet-code/](/vulnerabilities-identified-monero-multisignature-wallet-code/)
[^8]: https://libredd.it/r/Monero/comments/rlo8cz
