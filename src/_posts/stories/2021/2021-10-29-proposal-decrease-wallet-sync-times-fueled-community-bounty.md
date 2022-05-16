---
layout: post
category: story
title: Proposal to significantly decrease wallet sync times fueled by community bounty
description: "The Monero community has shown strong support for Koe's proposal to reduce scan times with 1-byte-per-output view tag by donating to Seth's bounty"
tags: bounties
image: 
last_modified_at: 15 November 2021
---

The Monero community has shown strong support[^1] for Koe[^2]'s proposal[^3] to reduce scan times with 1-byte-per-output view tag by donating to Seth[^4]'s bounty[^5]:

> [..] anyone can freely donate to incentivize and fund the work required [..] -Seth

A working demo of *view tags* can be found in Koe's Seraphis PoC branch[^6] (`view_scan.h`, `mock_sp_core_utils.h`[^7]).

This change is projected to significantly decrease wallet sync times by 50-70% without sacrificing privacy:

> I think we can easily reduce scanning by around 50-70% with 1 additional byte per output, call it the 'view tag’, a reduction even taking into account Janus. 

Furthermore, the increase in speed would also cover the scan time spent mitigating *Janus attacks*[^8]:

> [..] Janus might not increase scan times more than around 15-30% on average.[^9]

> [..] My recommendation is to roll this out in a hard fork alongside Janus [..] -Koe

Even with Janus accounted for and using the most conservative numbers, everyone using Monero wallets should still experience a decent speed increase. This would improve UX and potentially lead to an increase in adoption.

It is worth noting that, if implemented, this fix can **not** retroactively improve sync times. This aims to reduce wallet scan times of transactions created after the patch is implemented.

### Bounty payout criteria

- Code is open-source
- Code is submitted to the Monero repo as a pull-request
- Pull request properly improves wallet sync
- Pull request is accepted into Monero's code base after review

To start working on the project yourself, you should make your intentions public by posting a comment in the bounty's thread[^2].

Alternatively you can contribute some XMR to the bounty address posted by the *Monero Bounties Bot*. Your donation will be reflected in the comments.


```
Total Bounty: ~17.5 XMR (Oct 30, 2021)
```

---

**Update:**

- j-berman has started working on this bounty (PR ETA 2-4 weeks)[^5].

- PR #8061 submitted[^10].

---

[^1]: https://github.com/monero-project/research-lab/issues/73#issuecomment-954826429, https://nitter.net/sethforprivacy/status/1454087816716111884#m
[^2]: https://github.com/UkoeHB
[^3]: [https://github.com/monero-project/research-lab/issues/73](https://github.com/monero-project/research-lab/issues/73){:target="_blank"}{:rel="nofollow"}
[^4]: https://nitter.net/sethforprivacy
[^5]: [https://bounties.monero.social/posts/28/](https://bounties.monero.social/posts/28/){:target="_blank"}
[^6]: https://github.com/UkoeHB/monero/tree/seraphis_perf
[^7]: https://github.com/UkoeHB/monero/blob/seraphis_perf/tests/performance_tests/view_scan.h, https://github.com/UkoeHB/monero/blob/seraphis_perf/src/mock_tx/mock_sp_core_utils.h
[^8]: https://web.getmonero.org/2019/10/18/subaddress-janus.html
[^9]: https://github.com/monero-project/research-lab/issues/62#issuecomment-610758777
[^10]: https://github.com/monero-project/monero/pull/8061
