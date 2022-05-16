---
layout: post
category: story
title: Justin Berman posts 6th and final CCS progress report
description: Justin Berman has published his sixth and final CCS progress report, ready for community feedback.
tags: dev
image: 
---

Justin Berman[^1] has published the sixth and final progress report[^2] for his CCS proposal[^3]:

> **Hours worked: 92+** (tracked until Jan 20)

> **Total hours worked: 537+**[^4]

> Final update! The most significant things I worked on since last update were monero-lws subaddress support, the informal audit of monero-lws, and reviewing/providing feedback on JAMTIS (the next gen address scheme protocol).

### CCS work

- `monero-lws` subaddress support
- submitted proposal for adding subaddress support to the light wallet rest API[^5]
- submitted a first draft of the informal audit of `monero-lws`[^6]
- reviewed and provided feedback on *JAMTIS*, the new addressing scheme for Monero[^7]
- other/misc work (view tag implementation[^8]) 

### CCS conclusions

a) Improving the decoy selection algorithm

> Unfortunately, or fortunately rather, not too much was born out of my efforts in this area over the course of the CCS.

b) `monero-lws` informal audit

> My conclusion is that there are no obvious backdoors :)

> A user who is running monerod + monero-lws on a machine only the user has access to does not leak any information about their Monero transactions to a 3rd party through normal usage.[^9]

> In its current state, the review is not complete.

c) Subaddresses in `monero-lws`

> [..] it would likely make more sense to skip the simpler implementation, and go straight for the larger implementation. So I worked on and submitted this proposal[^10]. I plan to work on this to completion in another CCS.

Read the full progress report[^2] and the major highlights[^9] to learn more about Justin's contributions.

The dev is planning to submit a new CCS proposal *very soon*:

> In summary, I very much so enjoyed working full-time on Monero these past few months, and I hope to submit a new CCS very soon. I have deep gratitude for being granted the opportunity to contribute to Monero in this capacity. I feel very lucky and want to keep going 110%.

---

[^1]: https://github.com/j-berman
[^2]: [https://repo.getmonero.org/monero-project/ccs-proposals/-/merge_requests/249#note_14743](https://repo.getmonero.org/monero-project/ccs-proposals/-/merge_requests/249#note_14743){:target="_blank"}
[^3]: https://repo.getmonero.org/monero-project/ccs-proposals/-/merge_requests/249
[^4]: https://repo.getmonero.org/monero-project/ccs-proposals/uploads/cf61c2889d9ed87850ab2750aeac9823/CCS_1_time_tracking_update6.ods
[^5]: https://github.com/monero-project/meta/pull/647
[^6]: https://github.com/vtnerd/monero-lws/pull/29
[^7]: https://gist.github.com/tevador/50160d160d24cfc6c52ae02eb3d17024
[^8]: https://github.com/monero-project/monero/pull/8061
[^9]: [https://libredd.it/skjtjd/](https://libredd.it/skjtjd/){:target="_blank"}{:rel="nofollow"}
[^10]: https://github.com/monero-project/meta/pull/647
