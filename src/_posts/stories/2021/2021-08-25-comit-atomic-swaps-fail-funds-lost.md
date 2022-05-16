---
layout: post
category: story
title: MONT3M reports losing 0.03 BTC while attempting a BTC-XMR atomic swap using the COMIT tool
description: MONT3M loses 0.03 BTC while trying to complete a BTC-XMR atomic swap using the COMIT implementation 
tags: services
image: 
---

**MONT3M**[^1] reported[^2] that he lost 0.03 BTC while trying to complete a BTC-XMR atomic swap using the COMIT *swap* tool[^3].

As pointed out by **bordecraft**[^4], the most probable thing that happened is that the user failed to refund or cancel the swap after the 72 block timelock and the ASB operator published a *punish* transaction to claim the BTC.

A more technical explanation is available on the COMIT blog[^5]:

> Bob signs a punish transaction spending from Tx_cancel output to address_a, but which can only be published at time t_2. He shares this with Alice, to allow her to punish him by *taking the bitcoin in exchange for nothing*, in the case that Bob remains inactive for too long.

This behavior is normal and expected. In the end the only thing that can certainly be improved is the documentation and existing guides, as the community agrees it should be more clear that there is a risk of losing funds when doing an atomic swap, provided the user doesn't act in time.

Unfortunately, MONT3M took one for the team:

> I agree, unfortunately all the info sources I was using to complete the swaps (here, and here) didn't mention the punishment transaction or the 72 block window (at least that I saw).[^6]

And he shared some tips for new users:

> Do not initiate swaps in the evening, just in case things go wrong you can cancel and refund asap and dodge this punishment transaction.
Cancel and refund the swap if you get stuck waiting for Alice to lock the Monero
If you aren't tech savvy with a linux terminal (like me) don't mess around with large swaps that you would regret going wrong.

The community is sympathetic and would like to raise money[^7] to make up for his loss. 

If **MONT3M** reaches us to me I will publish his BTC address in this post for added visibility.


---

[^1]: https://libredd.it/user/MONT3M
[^2]: [https://libredd.it/r/Monero/comments/pb3f5a/sooo_i_lost_003_btc_trying_to_complete_an_atomic](https://libredd.it/r/Monero/comments/pb3f5a/sooo_i_lost_003_btc_trying_to_complete_an_atomic){:target="_blank"}{:rel="nofollow"}
[^3]: https://github.com/comit-network/xmr-btc-swap/releases
[^4]: https://libredd.it/user/bordecraft, https://libredd.it/r/Monero/comments/pb3f5a/sooo_i_lost_003_btc_trying_to_complete_an_atomic/ha9okwy/
[^5]: https://comit.network/blog/2020/10/06/monero-bitcoin/
[^6]: https://libredd.it/r/Monero/comments/pb3f5a/sooo_i_lost_003_btc_trying_to_complete_an_atomic/hab1xjr/
[^7]: https://libredd.it/r/Monero/comments/pb3f5a/sooo_i_lost_003_btc_trying_to_complete_an_atomic/haap069/
