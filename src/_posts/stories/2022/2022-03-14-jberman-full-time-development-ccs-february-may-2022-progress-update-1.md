---
layout: post
category: story
title: Justin Berman posts first progress report for Feb-May 2022 CCS proposal
description: "Justin Berman has published the first progress report for his Feb-May 2022 Monero dev work CCS proposal."
tags: dev
image: 
---

Justin Berman[^1] has published the first progress report[^2] for his Feb-May 2022 Monero dev work CCS proposal[^3]:

> **Hours worked: 285**

### CCS work overview

- identified and submitted patches for potential methods of fingerprinting MyMonero (PR 1[^4], PR 2[^5]) and `monero-lws` (PR[^6]) users by abnormal tx fees. 
- preliminary implementation of the background sync mode working (current branch[^7]).
- submitted a PR[^8] to bump ring size to 16
- submitted a PR to install `monero-lws` via a Dockerfile[^9]
- spent some time reviewing PR's (PR 1[^10], PR 2[^11])
[..]

To read the full report, consult the GH comment[^2].

---

[^1]: https://github.com/j-berman
[^2]: [https://repo.getmonero.org/monero-project/ccs-proposals/-/merge_requests/285#note_15356](https://repo.getmonero.org/monero-project/ccs-proposals/-/merge_requests/285#note_15356){:target="_blank"}
[^3]: https://repo.getmonero.org/monero-project/ccs-proposals/-/merge_requests/285
[^4]: https://github.com/mymonero/mymonero-core-cpp/pull/36
[^5]: https://github.com/mymonero/mymonero-core-cpp/pull/35
[^6]: https://github.com/vtnerd/monero-lws/pull/31
[^7]: https://github.com/j-berman/monero/tree/background-sync-mode
[^8]: https://github.com/j-berman/monero/tree/background-sync-mode	
[^9]: https://github.com/vtnerd/monero-lws/pull/30
[^10]: https://github.com/monero-project/monero/pull/8179
[^11]:https://repo.getmonero.org/monero-project/ccs-proposals/-/merge_requests/285
