---
layout: post
category: story
title: Self-replicating Monero nodes on the horizon with I2P torrenting
description: "Self-replicating Monero nodes are on the horizon, as the community restarts discussions to implement I2P torrenting capabilities into the Monero core software."
tags: dev
image: 
last_modified_at: 2021-11-25
---

Self-replicating Monero nodes are on the horizon, as the community restarts discussions to implement I2P[^0] torrenting capabilities into the Monero core software:

> Now that we have reproducible builds, we should work towards distributing this critical software in a decentralized way. 

carrington1859[^1] elaborates[^2]:

> By giving monerod the capability to seed the source code and/or compiled software, Monero nodes will become self-replicating and the Monero network will become more resilient.

> Integrated torrenting capabilities could also serve as an update mechanism for the core software.

A torrent-based distribution and update system would have other benefits as well:

- significantly lower maintenance burden
- reduced attack surface 
- less website development bottlenecks

I2P admin eyedeekay[^3] looks ready to get involved with the development:

> [..] I can help with this next month after the I2P release but it looks like there is still some UI/UX/Design decisions to make [..] How prepared are you guys for a PR to accomplish this?[^4]'[^5]

You can join the discussion on Github in *meta* issue #634[^2].

---

**Update: clarification, thanks to carrington (CDN is paid by Tari, not the GF; website general server costs the GF 2K/mo).**

---

[^0]: https://geti2p.net/en/
[^1]: https://github.com/carrington1859
[^2]: [https://github.com/monero-project/meta/issues/634](){:target="_blank"}{:rel="nofollow"}
[^3]: https://github.com/eyedeekay
[^4]: https://github.com/monero-project/monero-gui/issues/2274#issuecomment-976150834
[^5]: https://libera.monerologs.net/monero-community/20211123#c50133
