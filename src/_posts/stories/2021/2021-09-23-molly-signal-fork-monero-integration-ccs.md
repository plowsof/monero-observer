---
layout: post
category: story
title: Molly.im lead dev submits CCS proposal looking for community review
description: Signal fork for Android, Molly.im is looking to integrate Monero payments with this CCS proposal.
tags: CCS
image: 
last_modified_at: 17 October 2021
---

Oscar *valldrac* Mira[^1], the lead developer of Android Signal fork Molly.im[^2] has submitted a CCS proposal[^3] looking to integrate Monero payments with the app:

> The goal is to build a secure messaging app with integrated support for Monero payments and a decentralized backend.

> Monero features will include the ability to set up a XMR wallet, send and receive funds, keep track of the balance, and review the transaction history.

Currently there are two versions of the software available: Molly and Molly FOSS. The former uses Google proprietary code for some of the functionality.

If this proposal goes through, it looks like a third version of Molly will be developed, one that replaces MobileCoin[^4] with Monero:

> Build a flavor of Molly that replaces MobileCoin with Monero and connects to this server

The proposal suggests that users would be able to send and request XMR payments in-chat, view wallet seed, restore from seed, view transaction history and also transfer in/out.

It is worth noting that Molly fully depends on Signal's protocol/infrastructure, therefore Signal can potentially decide to ban Molly.im from connecting to their servers at any time in the future. 

valldrac explains:

> As we rely on the Signal for the server infrastructure we must adhere to Signal rules and limitations. All Molly features are improvements of the standard Signal client.

> Officially Signal takes the stance that they do not allow forks to connect to their servers. This has not always applied in practice since many projects exist that use their infrastructure. There is the risk, however, that Signal could at any time decide to enforce this policy in the future.

The proposal aims to deliver an *experimental but fully functional messaging app with XMR payments to the Monero community*, according to the lead dev: 

> This is not expected to scale to more than 10K simultaneous users and will not provide a production-ready or reliable service for end users. 

Total funding needed (Stage 1): $37,050 (in XMR).

ETA: ~18 weeks.

You can post your comments on Gitlab in !252[^3]. There's also a chat server available for Molly-related discussions on Matrix[^5].

---

**Update: proposal has been moved to the funding stage.**

---

[^1]: https://github.com/valldrac
[^2]: https://molly.im/, https://github.com/mollyim/mollyim-android
[^3]: [https://repo.getmonero.org/monero-project/ccs-proposals/-/merge_requests/252](https://repo.getmonero.org/monero-project/ccs-proposals/-/merge_requests/252){:target="_blank"}
[^4]: https://mobilecoin.com/
[^5]: #mollyim:matrix.org
