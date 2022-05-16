---
layout: post
category: story
title: xmrSale v2 released with support for random public nodes over tor
description: "xmrSale's anonymous developer has released v2 of the lightweight Monero payment processor, which comes with support for random public nodes over tor."
tags: merchants
image: 
---

xmrSale[^1]'s anonymous developer[^2] has released v2[^3] of the lightweight Monero payment processor, which comes with support for random public nodes over tor:

> With our latest update, we've made xmrsale even easier, more affordable and still private to run: [xmrsale v2] Lightweight Mode - Use random public nodes over tor

> xmrsale can now run without the requirement of hosting your own monero node.[^4]

### Changes

	Lightweight Mode - Use random public nodes over tor
    Streamlined setup command which creates wallet and displays seed
    Script monitoring wallet-rpc status
    Simplified configuration and startup UX
    Bug fixes, verbosity changes, doc updates

To learn more about the project, consult the associated CCS proposal[^5], the latest GH commits[^6]'[^7] and my previous report[^8].

To see xmrSale in action, check out the widget[^9] and the webstore[^10] demos.

Note that the project is still in *very early development* and the Docker image is currently broken.

The dev is planning to create installation videos and build additional e-commerce plugins for the software next.

---

[^1]: https://github.com/xmrsale/xmrSale
[^2]: https://github.com/xmrsale
[^3]: [https://repo.getmonero.org/monero-project/ccs-proposals/-/merge_requests/246#note_15294](https://repo.getmonero.org/monero-project/ccs-proposals/-/merge_requests/246#note_15294){:target="_blank"}
[^4]: https://libredd.it/tbia0l/
[^5]: https://repo.getmonero.org/monero-project/ccs-proposals/-/merge_requests/246
[^6]: https://github.com/xmrsale/xmrSale/commit/17676e527983ffd5e9b83c192132972342848f12
[^7]: https://github.com/xmrsale/xmrSale/commit/5c70a5f1dd9388f5b9662c145f64fffd14a910f4
[^8]: https://repo.getmonero.org/monero-project/ccs-proposals/-/merge_requests/246#note_11614
[^9]: [https://try.xmrsale.org/](https://try.xmrsale.org/){:target="_blank"}
[^10]: https://store.xmrsale.org/
