---
layout: post
category: story
title: Justin Berman publishes his 5th CCS progress report
description: Justin Berman has published his fifth CCS progress report, ready for community feedback.
tags: dev
image: 
---

Justin Berman[^1] has published the fifth progress report[^2] for his CCS proposal[^3]:

> Hours worked: ~104,  Total hours worked: 445

> Since last update, I spent most of my time working on view tags, which is the reason for the large gap since the prior update.

CCS work includes:

- completed work to get the wallet-side binning proposal in a state where it is open for feedback
- researched to better gauge how beneficial binning would be for users who spend multiple inputs in a single transaction, where their inputs are from older transactions that are close in age
- put together a very raw code snippet that demonstrates a way to implement a component of UkoeHB's deterministic ring selection
- finished reviewing and testing moneromoo's PR #7169
- reviewed yorha-0x's PR #8047
- researched atomic swaps further to better understand the requirements to get swaps working where XMR moves first

Justin plans to continue working on the issues listed in his initial progress report[^3], specifically: 

- Binning
- monero-lws subaddress support + informal audit
- Optimizing wallet scanning

---

[^1]: https://github.com/j-berman
[^2]: [https://repo.getmonero.org/monero-project/ccs-proposals/-/merge_requests/249#note_14390](https://repo.getmonero.org/monero-project/ccs-proposals/-/merge_requests/249#note_14390){:target="_blank"}
[^3]: https://repo.getmonero.org/monero-project/ccs-proposals/-/merge_requests/249
