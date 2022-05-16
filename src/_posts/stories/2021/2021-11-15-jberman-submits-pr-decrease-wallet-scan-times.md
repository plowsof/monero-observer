---
layout: post
category: story
title: j-berman submits PR to decrease wallet sync times
description: "j-berman has submitted a pull request which aims to reduce wallet scanning times for new Monero transactions by 30-40%."
tags: dev
image: 
last_modified_at: 2022-01-14
---

j-berman[^1] has submitted a pull request which aims to reduce wallet scanning times for new Monero transactions by 30-40%:

> Add view tags to outputs to reduce wallet scanning time #8061[^2]

> In tests on my machine, I saw reductions in scanning time upwards of 40% (and a minimum around 30%).

The code aims to implement view tags as proposed by Koe[^3] in MRL issue #73[^4], as previously reported[^5].

After conflicts are resolved and the PR is merged, j-berman should also be able to collect the associated bounty[^6].

---

**Update: add reference link to j-berman's comment[^7]; PR #8061 is now close to being merged.**

---

[^1]: https://github.com/j-berman
[^2]: [https://github.com/monero-project/monero/pull/8061](https://github.com/monero-project/monero/pull/8061){:target="_blank"}{:rel="nofollow"}
[^3]: https://github.com/UkoeHB
[^4]: https://github.com/monero-project/research-lab/issues/73
[^5]: [/proposal-decrease-wallet-sync-times-fueled-community-bounty/](/proposal-decrease-wallet-sync-times-fueled-community-bounty/)
[^6]: https://bounties.monero.social/posts/28
[^7]: https://github.com/monero-project/monero/pull/8061#issuecomment-1013368354
