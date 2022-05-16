---
layout: post
category: story
title: ArticMine and Isthmus weigh in on Rucknium's OSPEAD proposal feasibility
description: "Monero Core's ArticMine and MRL's Isthmus have weighed in on the feasibility of Rucknium's OSPEAD proposal in the latest #monero-research-lab meeting and on Github in !255."
tags: research
image: 
date: 2021-11-04 21:00
last_modified_at: 5 November 2021
---

Monero Core's ArticMine[^1] and *MRL*'s[^2] Isthmus[^3] have weighed in on the feasibility of Rucknium[^4]'s *OSPEAD*[^5] proposal in the latest *#monero-research-lab* meeting[^6] and on Github in !255[^7]. 

ArticMine suggested that there is merit in the OSPEAD approach and sees it as complementary to increasing *noise* via ring size increases/*binning*:

> I completed my feedback to OSPEAD [..] In summary I believe that the overall approach is feasible. I am waiting on Rucknium's modified plan. 

He also proposed postponing the implementation until the next hard fork, when the ring size will probably be increased from 11 to 16[^8]. That should provide enough data to finalize the research. 

Until that happens, Rucknium should be ready to submit a modified plan to ArticMine and release a version of his OSPEAD technical specification (*Document A*).

j-berman[^9] shared a summary of his suggestion to Rucknium:

> [..] use the real output data collected by Moser et al to fit a plausibly better distribution than the gamma distribution, using one of the multiple methods of fitting the distribution described in Document A [..]

Moments after the meeting, Isthmus shared his first impressions of OSPEAD on Github:

> [..] OSPEAD is a clever approach that will be an improvement over our existing decoy selection algorithm. However there may be an even better solution out there [..]

He went on to recommend additional research into potential alternatives to OSPEAD and analysis of tradeoffs before choosing the optimal solution:

> [..] this would add another week or two to the time and budget, but I believe that it will be worth every piconero to be confident that we're making the strongest move possible to protect Monero users.

Isthmus concluded the public message with a praise of Rucknium's recent efforts and some optimism for the future:

> I've collaborated with Rucknium over the past few months and have been very impressed with their work & technical skillset that is very well suited for this research.

> I am very thankful and relieved to see MRL resume ring signature research, and I look forward to seeing what we learn over the course of this initiative.

Even though OSPEAD has been meet with some early criticism[^10], the community seems to be warming up to the proposal. 

Most of the doubts would certainly be dispelled if all information about the attack were to be publicly released, as Isthmus suggested:

> I would lean towards ultimately releasing details about the attack, since restricting access to knowledge of the heuristic may hinder open-source researchers more than our adversaries.

Rucknium's OSPEAD is one of the main discussion topics on the upcoming November 10th MRL meeting agenda[^11].

---

[^1]: https://libredd.it/user/ArticMine
[^2]: https://github.com/monero-project/research-lab
[^3]: https://github.com/mitchellpkt
[^4]: https://github.com/Rucknium
[^5]: [https://repo.getmonero.org/monero-project/ccs-proposals/-/merge_requests/255](https://repo.getmonero.org/monero-project/ccs-proposals/-/merge_requests/255){:target="_blank"}{:rel="nofollow"}
[^6]: https://libera.monerologs.net/monero-research-lab/20211103#c43746
[^7]: https://repo.getmonero.org/monero-project/ccs-proposals/-/merge_requests/255#note_12497
[^8]: [/monero-research-lab-meeting-27-october-2021](/monero-research-lab-meeting-27-october-2021), https://libera.monerologs.net/monero-research-lab/20211020#c40230
[^9]: https://github.com/j-berman
[^10]: [/rucknium-ospead-ccs-proposal/](/rucknium-ospead-ccs-proposal/)
[^11]: [/monero-research-lab-meeting-10-november-2021/](/monero-research-lab-meeting-10-november-2021/)
