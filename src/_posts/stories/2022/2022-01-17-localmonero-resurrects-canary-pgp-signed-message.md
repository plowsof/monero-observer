---
layout: post
category: story
title: LocalMonero resurrects canary with new PGP-signed message
description: "LocalMonero has resurrected their warrant canary and this time it includes a more specific PGP-signed message."
tags: events
image: 
---

LocalMonero[^1] have *resurrected*[^2] their warrant canary[^3] and this time it includes a more specific PGP-signed message:

```
LocalMonero / AgoraDesk has, up to this date, received:
2 law enforcement requests for user information, of which
0 were served on us through the proper legal channels and resulted in
0 users' data being turned over
```

This comes as a reaction to recent controversy[^4] surrounding the implication of the *dead canary* ASCII art[^5] that has been sitting on LM's Canary page for *a long time*, according to Alex from LocalMonero:

> The dead bird just means we've received law enforcement requests. Doesn't mean anything else. The canary had been dead for a long time. Just so happens that it was noticed now.

> We, once again, apologize for the confusion caused by this, and we have now updated our canary based on the feedback we've received from the community over the past week.

The new canary message clearly specifies:

- how many LE requests they have received and how many of them resulted in a turn over of data
- whether they were coerced into installing backdoors or were otherwise compromised
- a timestamp and the latest Monero block hash

Users can verify that the message was signed by LocalMonero by importing their PGP key[^6] (fingerprint: 0D0D 0A3F F330 51FF A5C1  1577 3D7C 77D5 6D08 AED3).

LM plans to update the message at least once per 120 days. A failure to update the message could indicate the presence of a *gag order*[^7] that is legally  preventing them from updating the canary.

To learn more about the significance and inherent limitations of warrant canaries[^8], read EFF's Deeplinks Blog articles[^9]'[^10].

---

[^1]: https://localmonero.co
[^2]: [https://libredd.it/s6bmxy](https://libredd.it/s6bmxy){:target="_blank"}{:rel="nofollow"}
[^3]: [https://localmonero.co/canary](https://localmonero.co/canary){:target="_blank"}
[^4]: https://libredd.it/r/Monero/comments/s1qyf5/localmonero_dead_canary_the_dead_bird_just_means/hs9zx3r/?context=3
[^5]: https://nitter.net/btclovera/status/1480932335302455305
[^6]: https://keybase.io/localmonero/pgp_keys.asc?fingerprint=0d0d0a3ff33051ffa5c115773d7c77d56d08aed3
[^7]: https://wikiless.sethforprivacy.com/wiki/Gag_order
[^8]: https://wikiless.sethforprivacy.com/wiki/Warrant_canary
[^9]: https://www.eff.org/deeplinks/2016/05/canary-watch-one-year-later
[^10]: https://www.eff.org/deeplinks/2014/04/warrant-canary-faq
