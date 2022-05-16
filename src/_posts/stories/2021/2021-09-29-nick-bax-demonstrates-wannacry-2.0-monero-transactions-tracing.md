---
layout: post
category: story
title: Nick Bax demonstrates how XMR transactions related to WannaCry 2.0 were traced
description: Blockchain analyst Nick Bax published a detailed post where he demonstrates how Chainalysis was able to trace XMR transactions related to the WannaCry 2.0 malware.
tags: research
image: 
---

Blockchain analyst Nick Bax[^1] published a detailed post[^2] where he demonstrates how Chainalysis[^3] was able to trace XMR transactions related to the *WannaCry 2.0*[^4] malware:

> Wannacry 2.0: funds tracked from BTC to XMR and back to BTC and BCH after 3 months.

## Overview

- [12-15 May 2017] - WannaCry 2.0 ransomware initial outbreak (300K+ Windows machines infected[^5])
- [12 May 2017 at 07:44] - Marcus Hutchins discovers a kill-switch which prevented already infected machines from being encrypted[^6]
- [3 Aug 2017] - BTC converted to 820.79942522 XMR via ShapeShift
- [17 Aug 2017] - Shapeshift-received XMR consolidated in 3 transactions
- [Sep 2017] - Neutrino research team publish article on tracing Shapeshift BTC > XMR transactions[^7]
- [2 Nov 2017] - 536 XMR converted to BCH using ShapeShift in 9 transactions
- [19 Dec 2017] - Cyberattack blamed[^8] on *Lazarus Group*[^9]

In an attempt to obfuscate the source or destination of the funds, an attempted to convert them to a privacy-focused cryptocurrency has been made (BTC > XMR > BTC/BCH). Shapeshift and Changelly were used for some of the transactions.

Nick shares the info that he used to complete the trace:

- data from Neutrino’s article [^7]
- data from ShapeShift’s API[^10]
- data from XMRchain.info[^11]

Additional data can be found in the associated Github repository[^12].

## Trace factors

- the existence of *long payment IDs* (which have been deprecated[^13] and replaced with subaddresses in 2019)
- the user could select a low number of decoys per transaction (today it's fixed at 10, which increase privacy considerably)
- Monero CLI wallet users were isolated/profiled based on the number of allowed transaction outputs (currently not possible as both Monero GUI & Cake Wallet both allow multiple > 2 TXOs/tx)
- the use of centralized exchanges
- failed attempt at *churning*[^14]

The post concludes with a summary and some interesting things to consider:

> Nevertheless, this example shows that probabilistic analysis can lead to very high certainties in Monero tracing. It shows that even state-sponsored actors can be traced if improperly using Monero.

> The information from this leak can also potentially be used alongside other Monero attacks, such as the recently-described flood attack, to increase the reliability of EAE attacks.[^15]

## My advice

1. Use XMR peer-to-peer (as it was intedended to be used) whenever you can, don't go through a centralized exchange if you can help it.
2. Use Tor with GNU/Linux/Whonix/Qubes/Tails (deny metadata collection). Don't use Windows.
3. Reassess your treat model and revise your OPSEC accordingly.

---

[^1]: https://medium.com/@nbax
[^2]: [https://medium.com/@nbax/tracing-the-wannacry-2-0-monero-transactions-d8c1e5129dc1](){:target="_blabk"}{:rel="nofollow"}
[^3]: https://www.chainalysis.com/
[^4]: https://en.wikipedia.org/wiki/WannaCry_ransomware_attack
[^5]: https://en.wikipedia.org/wiki/WannaCry_ransomware_attack#cite_note-2
[^6]: https://en.wikipedia.org/wiki/WannaCry_ransomware_attack#cite_note-6
[^7]: https://www.neutrino.nu/Research_WannaShift_to_Monero.html
[^8]: https://en.wikipedia.org/wiki/WannaCry_ransomware_attack#cite_note-7
[^9]: https://en.wikipedia.org/wiki/Lazarus_Group
[^10]: https://shapeshift.io/txstat/18hjgJRmafRkJmGNiNDy9sEsERLw53ZWv3
[^11]: https://xmrchain.info/
[^12]: https://github.com/nickbax/wannacry_monero_tracing
[^13]: http://monerotoruzizulg5ttgat2emf4d6fbmiea25detrmmy7erypseyteyd.onion/2019/06/04/Long-Payment-ID-Deprecation.html
[^14]: https://monero.stackexchange.com/questions/4565/what-is-churning
[^15]: [/researchers-publish-forensic-statistical-analysis-xmr-transaction-volume-anomaly](/researchers-publish-forensic-statistical-analysis-xmr-transaction-volume-anomaly)
