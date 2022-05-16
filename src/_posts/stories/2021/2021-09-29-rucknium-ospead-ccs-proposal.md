---
layout: post
category: story
title: Rucknium submits sensitive CCS proposal aiming to fortify Monero against statistical attacks
description: Rucknium submits OSPEAD CCS proposal that aims to fortify Monero against statistical attacks.
tags: CCS
image: 
last_modified_at: 16 November 2021
---

Pseudonymous contributor Rucknium[^1] has submitted a CCS proposal[^2] that promises to fortify Monero against statistical attacks:

> The current mixin selection algorithm (MSA) has been acknowledged as a weak point in Monero's privacy model, but to date no plan has emerged to improve it. Over the last six weeks I have developed an outline of a plan to overhaul the algorithm through a technique I have termed OSPEAD: Optimal Static Parametric Estimation of Arbitrary Distributions. 

The proposed fix cannot be disclosed publicly at this point, due to the sensitive nature of the information it contains:

> A key difficulty with writing this CCS proposal is that the attack and the plan to overhaul the MSA have some indirect links. In other words, if I were to publicly fully specify the plan to overhaul the algorithm, a truly dangerous adversary --- such as a government agency or a criminal gang --- might be able to use some information in the plan to help develop its own attack against user privacy. 

j-berman[^3] will assist Rucknium to develop and implement OSPEAD, as outlined in his own CCS proposal[^4].

There are 3 milestones listed:

1. Deliver fully specified estimation plan to the scientific review panel (3 weeks)
2. Deliver initial probability density function to the scientific review panel (5 weeks)
3. Deliver final version of probability density function to Monero developers (2 weeks)

> After the scientific review panel examines the report and suggests improvements, a final version of the probability density function for the MSA will be produced.

> This finalized probability density function will be delivered to Monero developers for consideration to be included in a subsequent release of the Monero reference wallet.

Rucknium notes that the implementation of a new MSA should not require a hard fork.

> The 10 weeks of work will not be completely contiguous, but I expect Milestone 3 to be reached by January or February 2022. I will set the final expiration date for the proposal, for the purposes of the CCS proposal process, to July 2022.

Rucknium's previous contributions to the Monero ecosystem include:

- statistical contributions to the analysis of the mid-2021 Monero transaction volume anomaly, particularly on the subject of ring member age[^5]
- suggesting the development of a plan to recruit technical talent for the Monero Project[^6]

He is also involved in a few other cryptocurrency initiatives that may involve monetary compensation: BCH's *CashFusion Red Team*[^7] and the *Townforge* blockchain[^8] ecosystem.

```
Total funding needed: 171 XMR ($100/hr rate).

ETA: February/March 2022 (all milestones).
```

You can post your comments and questions on Gilab in !255[^2].

**UPDATE 9/30**

The fact that the proposal aims to keep some information confidential, mainly the method of choosing the probability distribution:

> The actual mixin selection algorithm will be publicly visible and open source in the Monero code. How the exact probability distribution was determined, however, should not be disclosed [..][^10]

has been viewed with skepticism[^9] by some community members:

> [..] I don't see how that would be acceptable.[^11]

> This is exactly how the NSA backdoor was put into DUAL_EC_DRBG: algorithm in plain view with "mystery constants" of unexplained provenance.[^12]

> What happens when this group determines the probability distribution in a way that is also harmful to privacy either by accident or on purpose? You can't only assume the convenient outcome in my eyes.[^13]

It is currently unclear if that info could/would be disclosed after OSPEAD implementation or if needs to stay away from the public *forever*:

> [..] it's unclear to me from reading this post and Reddit, but the statistical model/approach would be published after it is implemented in Monero and binaries are released, etc., correct?[^14]

Most Monero users would probably prefer everything is developed in the open, as that would produce the strongest possible code:

> I think open development is the strongest method of producing the strongest code. I would rather all methodologies opened up to everyone, for all to scrutinize, review, and join in collaboration.[^15]

The community is still reviewed the proposal. I will update this or create a new report if needed.

**UPDATE 11 November 2021**

The proposal was moved to the funding stage[^16].

**UPDATE 16 November 2021**

The proposal was fully funded[^17].

---

[^1]: https://repo.getmonero.org/Rucknium, https://github.com/Rucknium
[^2]: [https://repo.getmonero.org/monero-project/ccs-proposals/-/merge_requests/255](https://repo.getmonero.org/monero-project/ccs-proposals/-/merge_requests/255){:target="_blank"}, 
[^3]: https://repo.getmonero.org/j-berman
[^4]: https://ccs.getmonero.org/proposals/j-berman-3-months-full-time.html
[^5]: [/researchers-publish-forensic-statistical-analysis-xmr-transaction-volume-anomaly](/researchers-publish-forensic-statistical-analysis-xmr-transaction-volume-anomaly)
[^6]: https://libredd.it/r/Monero/comments/pkg3d6/the_monero_project_should_actively_recruit/
[^7]: https://flipstarter.redteam.cash/
[^8]: https://github.com/Rucknium/TownforgeR
[^9]: https://libredd.it/r/Monero/comments/py8ub3/ccs_proposal_ospead_fortifying_monero_against/
[^10]: https://libredd.it/r/Monero/comments/py8ub3/ccs_proposal_ospead_fortifying_monero_against/hetefog/?context=3
[^11]: https://libredd.it/r/Monero/comments/py8ub3/ccs_proposal_ospead_fortifying_monero_against/hestrdm/?context=3
[^12]: https://libredd.it/r/Monero/comments/py8ub3/ccs_proposal_ospead_fortifying_monero_against/hetwy2o/?context=3
[^13]: https://libredd.it/r/Monero/comments/py8ub3/ccs_proposal_ospead_fortifying_monero_against/hetpt2a/?context=3
[^14]: https://repo.getmonero.org/monero-project/ccs-proposals/-/merge_requests/255#note_11582
[^15]: https://repo.getmonero.org/monero-project/ccs-proposals/-/merge_requests/255#note_11583
[^16]: [/rucknium-ospead-ccs-proposal-funding](/rucknium-ospead-ccs-proposal-funding)
[^17]: https://ccs.getmonero.org/proposals/Rucknium-OSPEAD-Fortifying-Monero-Against-Statistical-Attack.html
