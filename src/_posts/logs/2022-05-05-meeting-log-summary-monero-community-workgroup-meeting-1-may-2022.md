---
layout: post
category: story
title: "Meeting summary: Monero Community Workgroup, 1 May 2022"
description: "This is a comprehensive summary, with added reference links, of the Monero Community Workgroup meeting from May 1st 2022, 1700 UTC."
tags: [logs]
image: 
meeting_name: "Monero Community Workgroup"
meeting_report: /monero-community-workgroup-meeting-1-may-2022/
meeting_date: "2022-05-01"
meeting_logs: /assets/logs/220501-community.log
date: 2022-05-05 17:00
---

This is a comprehensive summary, with added reference links, of the [Monero Community Workgroup meeting](/monero-community-workgroup-meeting-1-may-2022) from May 1st 2022, 1700 UTC.

## Logs

The raw, unedited, full log file for this meeting: 

[220501-community.log](/assets/logs/220501-community.log) (172 lines)

## Summary

*Note: it is possible that some relevant information may be missing from this summary; read the full log file for the complete, unedited discussion.*

- **Participants**: 7 (*plowsof[^1], monerobull[^2], cryptogrampy[^3], merope[^4], w[^5], Rucknium[^6], midipoet[^7]*)

- **(1) Community highlights**

	- (1.1) **on the upcoming v15 network update[^8]:**
	
	- plowsof mentioned Sethforprivacy's hardfork checklist[^9]
	
	- monerobull got a reply from Kraken support stating that *their developers will keep things up to date* [with the upcoming network update]
	
	- (1.2) **on malicious remote nodes tricking users into paying high fees[^10]:**
	
	- plowsof mentioned the malicious nodes that were causing trouble with high tx fees, the warning that was added to the Monero GUI wallet[^11] and the proposed long term fix (list of trusted nodes)
	
	- monerobull suggested including a fallback to random nodes
	
	- w argued against a fall back to random, citing malicious actors that would try to get on the auto-lists
	
	- merope jumped in to suggest taking advantage of the already trusted main seed nodes of the network that are used for bootstrapping the network
	
	- plowsof added that Feather wallet also has some list of nodes it performs health checks on 
	
	- cryptogrampy warned of a potential increase in reliance on the seeds
	
	- (1.3) **on the latest Monero GUI/CLI releases[^12]:**
	
	- plowsof reminded everyone to upgrade to the newest version, 0.17.3.2 

- **(2) CCS Ideas**

	- (2.1) **on spirobel's 'Monero Afghanistan Expansion Strategy' proposal**[^13]:
	
	- monerobull voted against
	
	- w expressed their skepticism about how this CCS could help an entire country
	
	- cryptogrampy suggested spirobel should reintroduce the proposal in a more palatable way in the future

  - (2.2) **on oeAdgK01's 'Translation of Monero GUI Wallet, CLI Wallet, monero-site, Behavioral Finance, Cryptocurrency Markets (subtitles), Moneropedia, User Guides to Greek' proposal**[^14]:

  - plowsof mentioned the ongoing problem related to the lack of reviewers

  - monerobull expressed their frustration with the current translation system that essentially renders translations that were already funded entirely worthless

  - (2.3) **on Moneroist's 'Patronero - Open Source project for donating by mining' proposal**[^15]:
	
  - monerobull voted against, expressing doubts about the practicality of the project: *who would ever download a miner to support someone*[?]

  - cryptogrampy suggested that a public api that uses an agreed upon shared database (git repo?) of public addresses people would like to receive donations at would be more useful than *a one off mining thing*

  - merope voted against, pointing to the extremely low profitability of mining: *unless the donor has a ton of hashrate, it won't be very useful*, and doubted the need for two separate apps which apparently serve the same function
	
  - Rucknium chimed in to state that *Patronero may cost more in CCS funds than it raises*
  
  - (2.4) **on willk's 'Monero business kit' proposal**[^16]:
  
  - cryptogrampy found the idea of a *an all in one docker deployable web shop* *very cool* but insisted on getting an answer on *why it should get community funded / why people need it over existing solutions*
  
  - w wondered if the proposer had any plans of monetizing the project
  
  - monerobull wondered if the requested funding was reasonable: *is that worth 100+ xmr*[?]
  
  - Rucknium stated that the proposal was *strongly improved from its initial draft* but it should *go out and get more engagement* 
  
  - (2.5) **on koe's 'Seraphis Wallet PoC 2 funding proposal'**[^17]:
  
  - w, merope, monerobull, plowsof, all voted for
  
- **(3) WiP CCS proposals**  

  - plowsof mentioned Rucknium's OSPEAD[^18] proposal in context of the recently set HF date
  
  - Rucknium confirmed that the timeline for OSPEAD is now more clear and the hard fork (and rise of ring size from 11 to 16) should help with the statistical estimation
  
  - plowsof has been *trying to re-unite funds from the CCS to their rightful owners*, looking to see if any of the devs are having issues[^19]
  
  - plowsof confirmed that hinto, maintainer of *monero-bash*[^20], has been paid out in full after completing all CCS milestones, and all other overdue payment issues were resolved
  
  - plowsof stated that m0n3r0d1c3's (proposer of the *Monero casino* CCS[^21]) IRC/Matrix connectivity issues should also be resolved soon
  
  - midipoet confirmed that they have received half of the funds as a payout and organised flight and hotel for Oslo[^22]
  
  - midipoet asked the community what type of educational material they should hand out at the event

- - **(4) Open Ideas**  

  - plowsof suggested adding --rpc-access-control-origins=* to a public node config to help the monero-javascript ecosystem
  
  - plowsof asked if anyone is interested in *podcasting 2.0* using Monero
  
  - merope suggested an idea for a potential future CCS proposal about promoting Monero in the UAE

- /end 
---

Let me know if you find this type of report helpful. If not, I will redirect time spent on this to other tasks.

Feedback, suggestions and edits always welcome @[/about](/about#signature).

**-3RA**

---

[^1]: https://github.com/plowsof
[^2]: https://libredd.it/user/monerobull
[^3]: https://github.com/CryptoGrampy
[^4]: @merope:matrix.org
[^5]: @w:matrix.org
[^6]: https://github.com/Rucknium
[^7]: https://github.com/midipoet
[^8]: [/monero-consensus-hard-fork-16-july-2022/](/monero-consensus-hard-fork-16-july-2022/)
[^9]: https://github.com/monero-project/meta/issues/690
[^10]: [/xmrmfjj2-tricked-paying-exorbitant-19.73-xmr-fee-malicious-remote-node/](/xmrmfjj2-tricked-paying-exorbitant-19.73-xmr-fee-malicious-remote-node/)
[^11]: https://github.com/monero-project/monero-gui/pull/3897
[^12]: [/monero-gui-v0.17.3.2-oxygen-orion-point-release-p2pool-mining-support/](/monero-gui-v0.17.3.2-oxygen-orion-point-release-p2pool-mining-support/)
[^13]: https://repo.getmonero.org/monero-project/ccs-proposals/-/merge_requests/282
[^14]: https://repo.getmonero.org/monero-project/ccs-proposals/-/merge_requests/296
[^15]: https://repo.getmonero.org/monero-project/ccs-proposals/-/merge_requests/310
[^16]: https://repo.getmonero.org/monero-project/ccs-proposals/-/merge_requests/311
[^17]: https://repo.getmonero.org/monero-project/ccs-proposals/-/merge_requests/314
[^18]: [/rucknium-ospead-ccs-proposal/](/rucknium-ospead-ccs-proposal/)
[^19]: [/plowsof/](/plowsof/)
[^20]: [/hinto-janaiyo-releases-monero-bash-v1.5-completes-ccs-proposal/](/hinto-janaiyo-releases-monero-bash-v1.5-completes-ccs-proposal/)
[^21]: [/m0n3r0d1c3-submits-ccs-proposal-deploy-monero-dice-casino/](/m0n3r0d1c3-submits-ccs-proposal-deploy-monero-dice-casino/)
[^22]: [/midipoet-submits-ccs-proposal-oslo-freedom-forum-attendance/](/midipoet-submits-ccs-proposal-oslo-freedom-forum-attendance/)
