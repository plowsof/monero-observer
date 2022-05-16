---
layout: post
category: story
title: "noot posts dev report for XMR-ETH atomic swaps project"
description: "noot has posted a development update for her XMR-ETH atomic swaps project."
tags: dev
image: 
---

noot[^1] has posted a development update[^2] for her XMR-ETH atomic swaps project[^3]:

> I wanted to give an update on the development progress of the ETH-XMR atomic swap project, as it's been a couple months since I first posted.

> The update decreases the cost to redeem funds from the contract by 25x!! The deployment cost is still high, but this will be addressed in the next steps.

### Progress

- finishing the implementation of the "unhappy path" ie. the refund path 
- implementation of `swapcli` (peer and existing offer discovery)
- implementation of `swaprecover` (fund recovery)
- refactor of the protocol and codebase to verify a secp256k1 key on-chain instead of an ed25519 key, and use a DLEq (discrete logarithm equality) proof to verify that the two keys correspond to the same secret (gas savings)
- tests for discovery, making/taking offers, and initiation of a swap
- set up a CI that checks that the code is linted and all tests pass
- changed the license to LGPL after finishing the required refactors

### Next steps

- more testing and documentation
- refactoring the swap contract to be a "factory" contract (reduce gas costs)
- pure Go implementation of the DLEq proof/verification
- a browser UI that displays the current available offers, and eventually integration with a browser-based Ethereum wallet (ie. metamask)

The associated CCS proposal[^4]'[^5] got fully funded today[^6], in less than 24 hours.

To learn more about the project, read !277[^4] and consult my previous report[^7].

---

[^1]: https://github.com/noot
[^2]: [https://libredd.it/s6f7sb/](https://libredd.it/s6f7sb/){:target="_blank"}{:rel="nofollow"}
[^3]: https://github.com/noot/atomic-swap
[^4]: https://repo.getmonero.org/monero-project/ccs-proposals/-/merge_requests/277/diffs
[^5]: https://ccs.getmonero.org/proposals/noot-eth-xmr-atomic-swap.html
[^6]: [/noot-xmr-eth-atomic-swaps-ccs-proposal-funding/](/noot-xmr-eth-atomic-swaps-ccs-proposal-funding/)
[^7]: [/noot-xmr-eth-atomic-swaps-ccs-proposal/](/noot-xmr-eth-atomic-swaps-ccs-proposal/)
