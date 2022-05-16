---
layout: post
category: story
title: Justin Berman publishes his third CCS progress report
description: Justin Berman has published his third CCS progress report, ready for community feedback.
tags: dev
image: 
---

Justin Berman[^1] shared his third progress report[^2] for his CCS proposal[^3] with the community:

> Weeks 5-6 [Sep 27 - Oct 10]
Hours worked: 91.2 hours
Total hours worked: 280.9

>  I focused mainly on decoy selection algorithm work these past 2 weeks (lots of focus on binning + updated openmonero).

Technical details related to his work during the past two weeks are listed in his report:

- worked on a PoC for "binning" in the decoy selection algorithm
- implemented the gamma-based decoy selection algorithm in openmonero
- created a new PR to decrease the recent spend window in the decoy selection algo
- made a bit more progress on monero-lws informal audit, but not much
- chatted with vtnerd on a strategy to support subaddresses in monero-lws

Justin plans to continue working on the issues listed in his initial progress report[^4] for the next 2 weeks:

> I'm optimistic I'll be able to make significant headway into (and finish) most stuff from the CCS proposal by the end of the 3-month period, except for a majority of the one-off tasks (but also hoping to get subaddress support in monero-lws done).

- Binning
- Complete informal audit of monero-lws
- Continue working on thread safety in the daemon RPC
- Subaddress support in monero-lws

---

[^1]: https://github.com/j-berman
[^2]: [https://repo.getmonero.org/monero-project/ccs-proposals/-/merge_requests/249#note_11700](https://repo.getmonero.org/monero-project/ccs-proposals/-/merge_requests/249#note_11700){:target="_blank"}
[^3]: https://repo.getmonero.org/monero-project/ccs-proposals/-/merge_requests/249
[^4]: [/jberman-ccs-progress-update-1](/jberman-ccs-progress-update-1)
