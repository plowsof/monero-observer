---
layout: post
category: story
title: "Trezor users exposed to unicode domain phishing attack"
description: "Trezor users have been exposed to an unicode domain phishing attack."
tags: [security, wallets]
image: trezor-phishing-email.png
last_modified_at: 2022-04-04
---

Trezor[^1] users have been exposed to an unicode domain phishing attack:

> A scam email warning of a data breach is circulating. Do not open any email originating from noreply@trezor.us, it is a phishing domain.[^2]

The email has a clear subject line (*Your Trezor Suite might be compromised*) and attempts to direct users to *fake* domains (`suite.trẹzor.com`/`suite.xn--trzor-o51b.com`/`trezor.us`) in order to download a bogus software update and steal their private seeds.

It appears that Trezor has been using a third party service (MailChimp[^3]) for their *opt-in* newsletter, which lead to this situation:

> We are investigating a potential data breach of an opt-in newsletter hosted on MailChimp.[^4]

> MailChimp have confirmed that their service has been compromised by an insider targeting crypto companies.[^5]

Sethforprivacy[^6] has admitted falling for this type of attack *for the first time ever*:

> Tonight I fell for a phishing email for the first time ever.[^7] 

> I wasn't affected at all, but I did raise an embarrassing false alarm on Twitter and apologize for that.[^8]

> Thankful for all those that corrected me and pointed out it was a phishing email.[^9]

A lot of Trezor users[^10]'[^11]'[^12] that have received the scam email are insisting that they have not opted into any newsletter, including Seth:

> Leaked from MailChimp, apparently, though I didn't sign up for any newsletters [..][^13]

Users that did not click the link in the email, download the bogus update or share the private seed were not affected.

It might be pragmatic to assume that all Trezor email addresses are already circulating in an email list somewhere, and thus compromised/a target for future attacks.

This is not the first time Trezor disappoints its users this year. Read my previous reports[^14]'[^15] to learn more about the *AOPP* fiasco.

---

[^1]: https://trezor.io/
[^2]: [https://nitter.net/Trezor/status/1510548489884815361#m](https://nitter.net/Trezor/status/1510548489884815361#m){:target="_blank"}{:rel="nofollow"}
[^3]: https://mailchimp.com
[^4]: https://nitter.net/Trezor/status/1510548489884815361#m
[^5]: https://nitter.net/Trezor/status/1510558771944333312#m
[^6]: https://nitter.net/sethforprivacy
[^7]: https://nitter.net/sethforprivacy/status/1510440372010377231#m
[^8]: https://nitter.net/sethforprivacy/status/1510440377341390848#m
[^9]: https://nitter.net/sethforprivacy/status/1510464437328781313#m
[^10]: https://nitter.net/BitKryten/status/1510557527385247749#m
[^11]: https://nitter.net/4n0n59461602/status/1510548975199395840#m
[^12]: https://nitter.net/baccapaglierina/status/1510557956080812032#m
[^13]: https://nitter.net/sethforprivacy/status/1510593967829798917#m
[^14]: [/trezor-under-fire-ditching-cypherpunk-ideals-swiss-finma-aml-requirements-aopp](/trezor-under-fire-ditching-cypherpunk-ideals-swiss-finma-aml-requirements-aopp)
[^15]: [/trezor-backtracks-promises-remove-aopp-support](/trezor-backtracks-promises-remove-aopp-support)
