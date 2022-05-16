---
layout: post
category: story
title: Justin Berman publishes his second CCS progress report
description: Justin Berman has published his second CCS progress report, ready for community feedback.
tags: dev
image: 
---

Justin Berman[^1] shared his second progress report[^2] for his CCS proposal[^3] with the community:

> Weeks 3-4 [Sep 13 - Sep 26]
Hours worked: 96.7
Total hours worked: 189.7

> I spent a fair amount of time researching and fleshing out ideas to move forward on decisions to improve the decoy selection algorithm, and I don't have much in way of PR's yet.

Technical details related to his work during the past two weeks are listed in his report:

- provided a PoC to validate ring member distributions at consensus
- pushed forward the decision on what to do with timelocks
- completed ~50% of the "informal audit" on monero-lws
- looked into subaddresses in monero-lws a bit more
- published the post-mortem of decoy selection algorithm bugs
- reviewed and tested ndorf's PR to fix bug in RPC get_transactions

The same list from Justin's first progress report[^4] is the planned work for the next 2 weeks:

- Push forward the binning solution to improve the decoy selection algo
- Complete informal audit of monero-lws
- Update openmonero & monero-lws to match wallet2's decoy selection algo
- Continue working on thread safety in the daemon RPC
- Subaddress support in monero-lws

---

[^1]: https://github.com/j-berman
[^2]: [https://repo.getmonero.org/monero-project/ccs-proposals/-/merge_requests/249#note_11572](https://repo.getmonero.org/monero-project/ccs-proposals/-/merge_requests/249#note_11572){:target="_blank"}
[^3]: https://repo.getmonero.org/monero-project/ccs-proposals/-/merge_requests/249
[^4]: [/jberman-ccs-progress-update-1](/jberman-ccs-progress-update-1)
