---
layout: post
category: story
title: Monero Research Lab meeting scheduled for 27 April 2022 1700 UTC
description: Monero Research Lab meeting scheduled for 27 April 2022 1700 UTC on irc/Matrix channels.
tags: [events, calendar]
meeting_name: MRL
meeting_date: 2022-04-27 (WED)
meeting_start: 17:00 UTC
meeting_irc: irc://irc.libera.chat/#monero-research-lab
meeting_matrix: https://matrix.to/#/#monero-research-lab:monero.social
meeting_logs: /assets/logs/220427-mrl.log
meeting_summary: /meeting-log-summary-monero-research-lab-meeting-27-april-2022
last_modified_at: 2022-05-06
---

The next Monero Research Lab[^1] meeting is scheduled to take place on Wednesday, April 27 2022 at 17:00 UTC.

The meeting should take place on IRC-Libera/Matrix[^2] in the #monero-research-lab channels.

### Agenda

- Increasing Seraphis address indices from 7 -> 16 bytes (and increasing the address tag MAC from 1 -> 2 bytes) (logs[^3], gist[^4])
- Revisit @tevador's idea to record account indices in the tx, to improve robustness of output recovery (logs[^5])
- Focus on Seraphis address schemes and hopefully reach some kind of decision (or get closer, maybe narrow down the choices to 2 or 3) (MRL#92[^6], tevador's JAMTIS[^7])
- Adaptive CPU regulation for improved mining performance (maxwellsdemon)
- Further analysis of July-Aug 2021 tx volume anomaly (logs[^8])
- Improvements to the mixin selection algorithm (MRL#86[^9], JBerman's update[^10], MRL#88[^11], Rucknium's OSPEAD[^12]) 
- Seraphis[^13]/Triptych[^14]/Lelantus Spark[^15]
[..]

~~Note that this meeting’s chairperson and agenda are yet to be confirmed. The *-meta* issue should be posted shortly.~~

Logs for the previous meeting are available on Github[^16].

This meeting's chairperson was UkoeHB[^17]. To view the full discussion topic list, consult #691[^18].

---

**Update 22/4/27: issue, agenda and logs[^19] available.**

**Update 22/5/6: summary for this meeting is now available[^20].**

---

[^1]: https://github.com/monero-project/research-lab
[^2]: irc://irc.libera.chat/#monero-research-lab (IRC), https://matrix.to/#/#monero-research-lab:monero.social (Matrix)
[^3]: https://libera.monerologs.net/monero-research-lab/20220425#c88396
[^4]: https://gist.github.com/tevador/50160d160d24cfc6c52ae02eb3d17024?permalink_comment_id=4144862#gistcomment-4144862
[^5]: https://libera.monerologs.net/monero-research-lab/20211230
[^6]: https://github.com/monero-project/research-lab/issues/92
[^7]: https://gist.github.com/tevador/50160d160d24cfc6c52ae02eb3d17024
[^8]: https://github.com/monero-project/meta/issues/621#issuecomment-948953655
[^9]: https://github.com/monero-project/research-lab/issues/86
[^10]: https://repo.getmonero.org/monero-project/ccs-proposals/-/merge_requests/249#note_11480
[^11]: https://github.com/monero-project/research-lab/issues/88
[^12]: https://ccs.getmonero.org/proposals/Rucknium-OSPEAD-Fortifying-Monero-Against-Statistical-Attack.html
[^13]: https://github.com/UkoeHB/Seraphis
[^14]: https://eprint.iacr.org/2021/1173
[^15]: https://github.com/cypherstack/triptych-multisig/blob/main/main.pdf
[^16]: https://libera.monerologs.net/monero-research-lab/20220420#c87004
[^17]: https://github.com/UkoeHB
[^18]: [https://github.com/monero-project/meta/issues/697](https://github.com/monero-project/meta/issues/697){:target="_blank"}{:rel="nofollow"}
[^19]: [220427-mrl.log](/assets/logs/220427-mrl.log)
[^20]: [/meeting-log-summary-monero-research-lab-meeting-27-april-2022/](/meeting-log-summary-monero-research-lab-meeting-27-april-2022/)
