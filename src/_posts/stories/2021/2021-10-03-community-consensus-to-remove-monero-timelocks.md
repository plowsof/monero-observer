---
layout: post
category: story
title: Community close to reaching consensus on Monero's timelocks deprecation
description: "After a year of research and discussions, the community is close to reaching consensus on what to do with Monero's timelocks (unlock_time) implementation."
tags: dev
image: 
---

After a year of research and discussions[^1], the community is close to reaching consensus on what to do with Monero's timelocks (`unlock_time`) implementation.

Here's a big picture of everything:

## The basics

Each XMR transaction has inputs and outputs: 

- Outputs are the amounts available for further spending. 

- Inputs are selected from `n` previous transaction outputs.

The `unlock_time` field is part of all XMR transactions and it dictates when a transaction's outputs can be spent again, depending on its value:

- a value of `0` means funds can be spent *immediately* (after the standard 10 block maturity period)
- if it's below `500'000'000`, it is interpreted as a block height and compared with the current block height
- values above `500'000'000` are interpreted as Unix time in seconds (relative to the local time of the monero node machine)

## Vulnerabilities

TheCharlatan[^2] has discovered vulerabilities linked to Monero's timelocks in April 2020, while reading through the C++ code comments:

> Monero inherited a largely uncommented source code from the original cryptonote developers. Particularly hazy areas are commented with either //TODO or //FIXME. 

He also urged others to review the code in an effort to identify other potential bugs:

> I would strongly recommend other security researchers to take a tour through these. There are roughly 120 TODOs and 30 FIXMEs left, so there may be more to find.

Recently (12 September), two of his HackerOne reports have been publicly disclosed:

- *Hardware Wallets Do Not Check Unlock Time* (#817245[^3])
- *Unix time unlock_time values have dangerous validation rules enabling a number of exploits* (#854726[^4])

He published 3 blog posts[^5] related to the issues, here are the TLDR's:

> A lack of unlock time verification on the monero hardware wallets could have allowed a compromised host to permanently lock up a user’s XMR after a transaction. Both Trezor and Ledger patched the issue.

> [..] transaction unlock_time values were interpreted with local time, allowing a host of non-critical exploits targeting the integrity of the blockchain.

Both Ledger and Trezor have patched the issue.

All the known issues have been patched in Monero v0.17.00. No evidence of actual issue-related harm towards user funds was found.

## Proposed fixes

Although the bugs have been fixed for some time, `unlock_time` is still detrimental to Monero user's privacy.

The community has been exploring a few possible solutions:

- 1 - Deprecate/remove timelocks
- 2 - Encrypt `unlock_time`
- 3 - Tweak/improve the current implementation

j-berman[^6] shared an overview of the pros and cons for each of the above in MRL issue #78[^7]. 

Valid use cases of `unlock_time` are rather limited, currently. The main ones seems to be its use as a proof of unspent funds and as a potential subscription model. 

Contrary to what some may believe, COMIT's XMR-BTC atomic swap implementations is not based on the existence of Monero timelocks, as suggested in their paper[^8].

## Notes

- timelocks can be re-added to Monero in the future, but it would more difficult to implement
- if the community decides to eliminate timelocks, this could happen in one of the next few hard forks
- it seems that `unlock_time` is also a barrier to a decoy selection binning[^9] implementation, according to j-berman[^10]

The community seems to be almost ready to deprecate timelocks altogether.

If you can think of any other valid use cases or compeling reasons for not removing `unlock_time` or if you have any other suggestions, you can still post a comment on Github[^11], Reddit[^12] and attend the next MRL & Dev meetings[^13].


---

[^1]: https://github.com/monero-project/meta/issues/519, https://github.com/monero-project/meta/issues/610, https://github.com/monero-project/meta/issues/613, https://github.com/monero-project/meta/issues/614
[^2]: https://github.com/TheCharlatan
[^3]: https://hackerone.com/reports/817245
[^4]: https://hackerone.com/reports/854726
[^5]: https://thecharlatan.ch/Wallet-Timelock/, https://thecharlatan.ch/Monero-Unlock-Time-Vulns/, https://thecharlatan.ch/Monero-Unlock-Time-Privacy/
[^6]: https://github.com/j-berman
[^7]: https://github.com/monero-project/research-lab/issues/78#issuecomment-924622985 
[^8]: https://arxiv.org/pdf/2101.12332.pdf
[^9]: https://github.com/monero-project/research-lab/issues/84
[^10]: https://github.com/monero-project/research-lab/issues/86
[^11]: [https://github.com/monero-project/research-lab/issues/78](https://github.com/monero-project/research-lab/issues/78){:target="_blank"}{:rel="nofollow"}
[^12]: [https://libredd.it/r/Monero/comments/q0oiln/proposal_to_remove_timelock_feature/](https://libredd.it/r/Monero/comments/q0oiln/proposal_to_remove_timelock_feature/){:target="_blank"}{:rel="nofollow"}
[^13]: [/monero-research-lab-meeting-6-october-2021](/monero-research-lab-meeting-6-october-2021), [/monero-development-workgroup-meeting-17-october-2021](/monero-development-workgroup-meeting-17-october-2021)

