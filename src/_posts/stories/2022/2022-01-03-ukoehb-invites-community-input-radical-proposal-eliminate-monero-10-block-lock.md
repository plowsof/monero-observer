---
layout: post
category: story
title: "UkoeHB invites community input on radical proposal to eliminate Monero's '10-block-lock'"
description: "UkoeHB has invited the community to discuss a rather radical proposal to eliminate Monero's 10-block-lock security mechanism."
tags: research
image: 
last_modified_at: 2022-01-08
---

MRL's UkoeHB[^1] has invited the community to discuss a rather radical proposal[^2] to eliminate Monero's *10-block-lock* security mechanism:

> This is a proposal for eliminating Monero's 10-block-lock, which prevents users from spending outputs until they are 10 blocks old.

> If you are reading this, please first look at it academically before dismissing it out of hand. Yes, the drawbacks may be too severe, but before passing final judgement I would like a useful discussion.

### Proposal

- Allow transactions to have inputs with zero decoys if those inputs are very young (recently added to the chain).
- After a grace period, remove outputs from the pool of eligible ring members if they have been spent in a zero-decoy input.

If implemented, this would be a major change for the Monero ecosystem. 

Exchanges like Localmonero and Haveno would be able to deliver a better UX as users would not have to wait 10 blocks (~20 minutes) before spending the received coins.

However, there are some real drawbacks that the community needs to evaluate first:

- When a transaction is constructed, any decoys selected from the most recent ~20 eligible blocks may become provably spent.
- Since input-type-eligibility changes as a function of the block height where a tx gets mined, if a tx lingers in the tx pool for longer than the 20-block grace period, it may become invalid. 

This is obviously a compromise between usability and privacy:

> This offers a compromise between fast-spends and minimizing the damage those fast-spends can do to ring signature effectiveness.

But would a change so radical also eliminate Monero's *privacy by default* property and is this indeed a step in the right direction from a cypherpunk perspective?

The discussion is on-going. Post your comments on Github in MRL #95[^2].

---

**Update: tevador[^3] explores *Dummy transaction inputs*[^4] idea to mandate all transactions to have 16 outputs.**

**Update 1/8: add link to ArticMine's perspective (on Monerotopia Ep.47)[^5].**

---

[^1]: https://github.com/UkoeHB
[^2]: [https://github.com/monero-project/research-lab/issues/95](https://github.com/monero-project/research-lab/issues/95){:target="_blank"}{:rel="nofollow"}
[^3]: https://github.com/tevador
[^4]: https://github.com/monero-project/research-lab/issues/96
[^5]: https://piped.kavin.rocks/watch?v=O_tdF-McAFM (57:00)
