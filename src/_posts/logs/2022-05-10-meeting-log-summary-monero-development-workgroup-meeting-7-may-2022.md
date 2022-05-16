---
layout: post
category: story
title: "Meeting summary: Monero Development Workgroup, 7 May 2022"
description: "This is a comprehensive summary, with added reference links, of the Monero Development Workgroup meeting from May 7th, 2022, 1700 UTC."
tags: [logs]
image: 
meeting_name: "Monero Development Workgroup"
meeting_report: /monero-development-workgroup-meeting-7-may-2022
meeting_date: "2022-05-07"
meeting_logs: /assets/logs/220507-dev.log
---

This is a comprehensive summary, with added reference links, of the [Monero Development Workgroup meeting](/monero-development-workgroup-meeting-7-may-2022) from May 7th 2022, 1700 UTC.

### Logs

The raw, unedited, full log file for this meeting: 

[220507-dev.log](/assets/logs/220507-dev.log) (92 lines)

### Summary

*Note: it is possible that some relevant information may be missing from this summary; read the full log file for the complete, unedited discussion.*

- **Participants**: 8 (*UkoeHB[^1], selsta[^2], jberman[^3], ErCiccione[^4], rbrunner[^5], sech1[^6], hyc[^7], garth[^8]*)

- **(1) Network update: situation**

	- ErCiccione mentioned UkoeHB's *Multisig: signature fixes* #8149 PR[^9]
	
	- UkoeHB suggested vtnerd could potentially review #8149 before merging it
	
	- UkoeHB mentioned that *multisig: add post-kex verification round* #8220 PR[^10] is in the merge queue
	
	- hyc stated that the gitian arm macosx should be ready to merge before then
	
	- ErCiccione reminded everyone that everything should be ready by May 16th, as previously established[^11]
	
	- rbrunner and jberman have almost finished reviewing #8076[^12]
	
	- jberman thinks #7760[^13] could also be included, if he can review it in time
	
	- selsta reminded everyone that *this "feature complete" date was never really strict* and PRs can still be merged after May 16th
  
  - UkoeHB answered garth's question after clarifying that the multisig fixes are not consensus-breaking changes
  
  - garth thought that non-consensus breaking upgrades should not be listed in the *already pretty long* network upgrade history
  
- **(2) Decide stagenet fork date/height**

  - selsta suggested that the stagenet fork *is usually 1 week before mainnet* (July 9th)
  
  - jberman volunteered to handle the pull request and set the block height for the testnet fork (1982800 and 1983520)
  
  - ErCiccione summed up the definitive plan:

	-	```
		Branch/feature complete: May 16th, 2022
		Release date: June 16th, 2022
		Testnet hard-fork: May 16th, 2022, block 1982800 and 1983520
		Stagenet hard-fork: July 9th
		Mainnet hard-fork: July 16th, 2022, block 2668888
		```

---

Let me know if you find this kind of report helpful. If not, I will redirect time spent on this to other tasks.

Feedback, edits always welcome @[/about](/about#signature).

**-3RA**

---

[^1]: https://github.com/UkoeHB
[^2]: https://github.com/selsta
[^3]: https://github.com/j-berman
[^4]: https://github.com/erciccione
[^5]: https://github.com/rbrunner7/
[^6]: https://github.com/SChernykh
[^7]: https://github.com/hyc
[^8]: https://github.com/garth-xmr
[^9]: https://github.com/monero-project/monero/pull/8149
[^10]: https://github.com/monero-project/monero/pull/8220
[^11]: https://github.com/monero-project/meta/issues/630
[^12]: https://github.com/monero-project/monero/pull/8076
[^13]: https://github.com/monero-project/monero/pull/7760







