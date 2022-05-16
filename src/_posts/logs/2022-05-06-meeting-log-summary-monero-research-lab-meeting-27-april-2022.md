---
layout: post
category: story
title: "Meeting summary: Monero Research Lab, 27 April 2022"
description: "This is a comprehensive summary, with added reference links, of the Monero Research Lab meeting from April 27th, 2022, 1700 UTC."
tags: [logs]
image: 
meeting_name: "Monero Research Lab"
meeting_report: /monero-research-lab-meeting-27-april-2022
meeting_date: "2022-04-27"
meeting_logs: /assets/logs/220427-mrl.log
---

This is a comprehensive summary, with added reference links, of the [Monero Research Lab meeting](/monero-research-lab-meeting-27-april-2022) from April 27th 2022, 1700 UTC.

### Logs

The raw, unedited, full log file for this meeting: 

[220427-mrl.log](/assets/logs/220427-mrl.log) (108 lines)

### Summary

*Note: it is possible that some relevant information may be missing from this summary; read the full log file for the complete, unedited discussion.*

- **Participants**: 10 (*UkoeHB[^1], selsta[^2], jberman[^3], xmr-ack[^4], mj-xmr[^5], Rucknium[^6], cryptogrampy[^7], kayabaNerve[^8], merope[^9], gingeropolous[^10]*)

- **(1) Updates**

	- (1.1) **on Seraphis[^11]:**
	
	- UkoeHB implemented binned reference sets and plans to work on the 16/2 jamtis address index discussion/possible implementation, then discretized fees 
	
	- (1.2) **on statistical analysis**:
	
	- mj-xmr reported progress with the decoy selection algo analysis[^12], having summarized both the results and the strategy, and is planning to perform statistical analysis with Rucknium and jberman
	
	- mj-xmr mentioned the next (parallel) task of simulating the behavior of the system (fee and block size) in case of a sudden increase of transactions
	
	- Rucknium is working on estimating the effect (if any) of Minexmr's increase in its pool fee from 1.0% to 1.1% on April 1st[^13]
	
	- (1.3) **on view tags and security**:
	
	- jberman added support for view tags to the block explorer + monero-lws, helped add support for view tags to monero-python, and helped patch a vulnerability reported by kayabaNerve[^14]
	
- **(2) Larger JAMTIS[^15] address tags (and address indices)**
	
	- UkoeHB explained the address tag's MAC and how *increasing the size from 8 -> 18 will increase the blowfish ciphers from 1 to 3, but increasing the mac from 1 -> 2 bytes will reduce the cost of filter-failures by 1/256*
	
	- jberman pointed out that 10 bytes per output would *probably be more significant if the idea to have all tx's use 16 outputs was implemented*[^16]
	
	- UkoeHB mentioned plans to do *performance tests comparing 7/1 vs 16/2 jamtis address tags* (size in bytes)
	
- **(3) Ending comments**

  - cryptogrampy mentioned HotShop[^17]
  
  - selsta was looking for someone to do an updated multisig writeup of the cryptography that should help the next audit (preferably before the launch of Haveno)
  
  - Rucknium suggested MAGIC[^18] could help fund the writeup and audit, and pinged coinstudent2048
  
  - jberman pinged dangerousfreedom for the task
  
  
---

Let me know if you find this kind of report helpful. If not, I will redirect time spent on this to other tasks.

Feedback, edits always welcome @[/about](/about#signature).

**-3RA**

---

[^1]: https://github.com/UkoeHB
[^2]: https://github.com/selsta
[^3]: https://github.com/j-berman
[^4]: https://github.com/ACK-J
[^5]: https://github.com/mj-xmr
[^6]: https://github.com/Rucknium
[^7]: https://github.com/CryptoGrampy
[^8]: https://github.com/kayabaNerve
[^9]: @merope:matrix.org
[^10]: https://github.com/Gingeropolous
[^11]: [/ukoehb-submits-second-seraphis-wallet-poc-ccs-proposal/](/ukoehb-submits-second-seraphis-wallet-poc-ccs-proposal/)
[^12]: https://github.com/mj-xmr/monero-mrl-mj/tree/decoy/decoy
[^13]: [/minexmr-top-monero-pool-hashrate-drops-from-50-to-38-percent/](/minexmr-top-monero-pool-hashrate-drops-from-50-to-38-percent/)
[^14]: [/kayabanerve-discovers-security-vulnerability-monero-python-module/](/kayabanerve-discovers-security-vulnerability-monero-python-module/)
[^15]: https://gist.github.com/tevador/50160d160d24cfc6c52ae02eb3d17024
[^16]: https://github.com/monero-project/research-lab/issues/96
[^17]: [/cryptogrampy-submits-ccs-proposal-hotshop-monero-pos/](/cryptogrampy-submits-ccs-proposal-hotshop-monero-pos/)
[^18]: [/magic-monero-fund-starts-accepting-research-grant-applications/](/magic-monero-fund-starts-accepting-research-grant-applications/)










