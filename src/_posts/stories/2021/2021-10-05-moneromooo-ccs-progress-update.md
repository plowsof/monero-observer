---
layout: post
category: story
title: moneromooo shares his latest CCS progress report
description: moneromooo has shared a progress report for his latest CCS proposal to work on Monero.
tags: dev
image: 
---


moneromooo[^1] has shared the latest progress report[^2] for his CCS proposal[^3] to work on Monero:

> work on embedding encrypted data in bulletproofs [1]

> some more work on ArticMine's fee changes (ready now)

> [1] this actually ended up badly since it turns out the recipient is unable to decrypt it without info that leaks the index of the real spend, which we do not want - however, triptych will be able to embed 31 bytes this way without this drawback; moreover bulletproofs can still embed this data for retrieval by the sender only, since they already know the real spend

Since December 2020, he estimates having spent a total of 397 hours of work so far (out of his 520[^4] target).

moneromooo is a very well-known contributor, having worked for Monero in the past on multiple occasions[^5] over the years.

---

[^1]: https://github.com/moneromooo-monero
[^2]: [https://repo.getmonero.org/monero-project/ccs-proposals/-/merge_requests/192#note_11631](https://repo.getmonero.org/monero-project/ccs-proposals/-/merge_requests/192#note_11631){:target="_blank"}
[^3]: https://repo.getmonero.org/monero-project/ccs-proposals/-/merge_requests/192
[^4]: https://repo.getmonero.org/monero-project/ccs-proposals/-/merge_requests/192#note_10652
[^5]: https://repo.getmonero.org/monero-project/ccs-proposals/-/merge_requests/103, https://repo.getmonero.org/monero-project/ccs-proposals/-/merge_requests/75, https://repo.getmonero.org/monero-project/ccs-proposals/-/merge_requests/46, https://forum.getmonero.org/6/ideas/91206/moneromooo-january-march-coding
