---
layout: post
category: story
title: Monero Research Lab meeting scheduled for 9 March 2022 1700 UTC
description: Monero Research Lab meeting scheduled for 9 March 2022 1700 UTC on irc/Matrix channels.
tags: [events, calendar]
meeting_name: MRL
meeting_date: 2022-03-09 (WED)
meeting_start: 17:00 UTC
meeting_irc: irc://irc.libera.chat/#monero-research-lab
meeting_matrix: https://matrix.to/#/#monero-research-lab:monero.social
meeting_logs: https://github.com/monero-project/meta/issues/672#issuecomment-1063189000
last_modified_at: 2022-03-09
---

The next Monero Research Lab[^1] meeting is scheduled to take place on Wednesday, March 9th 2022 at 17:00 UTC.

The meeting should take place on IRC-Libera/Matrix[^2] in the #monero-research-lab channels.

### Agenda

- Fee policy and dynamic block size discussion for upcoming hard fork (meta#630[^3], #7819[^4], MRL#70[^5])
- Revisit @tevador's idea to record account indices in the tx, to improve robustness of output recovery (logs[^6])
- Focus on Seraphis address schemes and hopefully reach some kind of decision (or get closer, maybe narrow down the choices to 2 or 3) (MRL#92[^7], tevador's JAMTIS[^8])
- Adaptive CPU regulation for improved mining performance (maxwellsdemon)
- Further analysis of July-Aug 2021 tx volume anomaly (logs[^9])
- Improvements to the mixin selection algorithm (MRL#86[^10], JBerman's update[^11], MRL#88[^12], Rucknium's OSPEAD[^13]) 
- Seraphis[^14]/Triptych[^15]/Lelantus Spark[^16]
[..]

~~Note that this meeting's chairperson and agenda are yet to be confirmed.~~

This meeting's chairperson will be UkoeHB[^17]. To view the full discussion topic list and propose an agenda item, post a comment on Github in #672[^18].

Logs for the previous MRL meeting are available on Github[^19].

---

**Update: logs for this meeting are now available[^20].**

**Meeting notes:**

- UkoeHB has rebased `seraphis_lib` onto master and started working on multisig seraphis txs
- jberman has been working on background sync mode mostly
- Rucknium proposed discussing the effect of minexmr's upcoming fee change from 1% to 1.1% (an empirical estimate) and encouraged people to add thoughts about the paper[^21] linked by atomfried to MoneroResearch.info[^22]

---

[^1]: https://github.com/monero-project/research-lab
[^2]: irc://irc.libera.chat/#monero-research-lab (IRC), https://matrix.to/#/#monero-research-lab:monero.social (Matrix)
[^3]: https://github.com/monero-project/meta/issues/630
[^4]: https://github.com/monero-project/monero/pull/7819
[^5]: https://github.com/monero-project/research-lab/issues/70
[^6]: https://libera.monerologs.net/monero-research-lab/20211230
[^7]: https://github.com/monero-project/research-lab/issues/92
[^8]: https://gist.github.com/tevador/50160d160d24cfc6c52ae02eb3d17024
[^9]: https://github.com/monero-project/meta/issues/621#issuecomment-948953655
[^10]: https://github.com/monero-project/research-lab/issues/86
[^11]: https://repo.getmonero.org/monero-project/ccs-proposals/-/merge_requests/249#note_11480
[^12]: https://github.com/monero-project/research-lab/issues/88
[^13]: https://ccs.getmonero.org/proposals/Rucknium-OSPEAD-Fortifying-Monero-Against-Statistical-Attack.html
[^14]: https://github.com/UkoeHB/Seraphis
[^15]: https://eprint.iacr.org/2021/1173
[^16]: https://github.com/cypherstack/triptych-multisig/blob/main/main.pdf
[^17]: https://github.com/UkoeHB
[^18]: [https://github.com/monero-project/meta/issues/672](https://github.com/monero-project/meta/issues/672){:target="_blank"}{:rel="nofollow"}
[^19]: https://github.com/monero-project/meta/issues/669#issuecomment-1057212758
[^20]: https://github.com/monero-project/meta/issues/672#issuecomment-1063189000
[^21]: https://iacr.org/cryptodb/data/paper.php?pubkey=3172
[^22]: https://moneroresearch.info
