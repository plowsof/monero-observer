---
layout: post
category: story
title: Monero community torn between Seraphis/Lelantus Spark and Triptych
description: Monero community is torn between Seraphis/Lelantus Spark and Triptych
tags: research
image: 
last_modified_at: 19 Sep 2021
---

Between the various topics discussed during today's *Monero Research Lab* meeting[^1], the *Seraphis/Lelantus Spark vs Triptych* debate was arguably the most intriguing.

Lelantus Spark[^2] is the successor of Lelantus v1/v2. Most of the work is credited to Aram Jivanyan from Firo[^3]'s research team and Aaron Feickert from Cypher Stack[^4]. Aaron is on a full time contract with Firo.

The mere mention of Firo/CypherStack seems to have brought back flashbacks to previous controversies[^5], at least for some people:

> Who is behind this project ? There's a lot of "Firo" in the PDF, makes me wonna throw up to be honest..[^6]

> Is monero copying the technology from firo????[^7]

During the MRL irc meeting, sentiment appeared to shift in favor of switching to Seraphis rather than continuing to pursue Triptych, but the community still had a lot of questions. 

One of the biggest concerns is that XMR users would need to get new Lelantus Spark/Seraphis addresses. This could impact users, vendors and the general UX.

Although newly generated addresses wouldn't be affected, the address format change would effectively render previously widely published static addresses (donations, address book, etc) effectively unusable/invalid.

UkoeHB[^8] has been working on a PoC for Seraphis for the past couple of weeks and with the protocol still in the experimental stage and not implemented yet, the more eyes on it, the better for everyone. He shares some insight into the positives of Seraphis over Triptych:

> [..] membership proof delegation (allows tx chaining, offloading membership proofs to third parties, reduces timing analysis of slow tx like multisig), collaborative funding (multiple funders for a tx without big crypto design effort), better address schemes (several variations)

> If Seraphis/etc. turn out to be flops, Triptych is the best known protocol.[^9]

coinstudent2048[^10] has put together a technical report[^11] on Seraphis. He has been working on Seraphis's security proofs and is looking for community feedback for his formalization of the security properties[^12].

The community hasn't yet reached consensus in this matter, but both Triptych and Seraphis are at least *a year + out*[^13] in the future. 

We will know more after the next few meetings: 

- the MRL meeting, scheduled for 22 September, 2021 at 1700 UTC on irc/Matrix in the #monero-community[^15] channels.

- the dev meeting, which should take place on October 3rd, 2021 at 1700 UTC in the #monero-dev[^14] irc/Matrix channel. The consensus changes for the next hard fork are top priority for this discussion.

---

[^1]: https://github.com/monero-project/meta/issues/610, https://libera.monerologs.net/monero-research-lab/20210915
[^2]: [https://ia.cr/2021/1173](){:target="_blank"}{:rel="nofollow"}, https://yewtu.be/watch?v=vEZC1fTYRZk (video)
[^3]: https://firo.org/
[^4]: https://www.cypherstack.com/
[^5]: [/rehrar-removed-core-team/](/rehrar-removed-core-team/)
[^6]: https://libredd.it/r/Monero/comments/posi9i/lelantus_spark_secure_and_flexible_private/hcyv7s3/?context=3
[^7]: https://libredd.it/r/Monero/comments/posi9i/lelantus_spark_secure_and_flexible_private/hcyzoku/?context=3
[^8]: https://github.com/UkoeHB/monero/tree/seraphis_perf
[^9]: https://libera.monerologs.net/monero-research-lab/20210915#c27831	
[^10]: https://github.com/coinstudent2048
[^11]: https://raw.githubusercontent.com/coinstudent2048/writeups/main/seraphis.pdf
[^12]: https://github.com/UkoeHB/Seraphis/issues/2#issuecomment-918639450
[^13]: https://libera.monerologs.net/monero-research-lab/20210915#c27791, https://libera.monerologs.net/monero-research-lab/20210915#c27805
[^14]: irc://irc.libera.chat/#monero-dev (irc), https://matrix.to/#/#monero-dev:matrix.org (matrix)
[^15]: irc://irc.libera.chat/#monero-community (irc), https://matrix.to/#/#monero-community:monero.social (matrix)
