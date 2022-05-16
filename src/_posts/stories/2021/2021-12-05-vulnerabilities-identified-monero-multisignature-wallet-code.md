---
layout: post
category: story
title: Vulnerabilities identified in Monero multisignature wallet code
description: "According to Monero Core Team member binaryFate, some vulnerabilities have been identified in the implementation of Monero multisignature wallets code."
tags: [security, pinned]
image: 
last_modified_at: 2021-12-15
---

According[^0] to Monero Core Team member binaryFate[^1], some vulnerabilities have been identified in the implementation of Monero multisignature wallets code:

> These vulnerabilities affect (i) multisignature wallet creation and (ii) multisignature transaction signing. They can lead to funds being stolen by one of the signing parties.

Until a fix is released, it is **not recommended** for users to perform any multisignature transaction unless all signing parties can be trusted:

> If all signing parties cannot be trusted, no transaction should be attempted. Funds are not at risk if they are not moved and if the wallet-creation process was not abused.

The vulnerabilities were initially disclosed and discussed via the *Vulnerability Response Process*[^2].

---

**Update: added link to getmonero.org announcement[^0].**

**Update 12/15: multisig fixes PR #8114 submitted (not yet merged)[^3].**

---

[^0]: [https://www.getmonero.org/2021/12/06/vulnerability-multisig.html](https://www.getmonero.org/2021/12/06/vulnerability-multisig.html){:target="_blank"}
[^1]: https://github.com/binaryFate
[^2]: https://github.com/monero-project/meta/blob/master/VULNERABILITY_RESPONSE_PROCESS.md
[^3]: https://github.com/monero-project/monero/pull/8114/files
