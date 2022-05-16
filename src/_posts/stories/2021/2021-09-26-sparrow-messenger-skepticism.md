---
layout: post
category: story
title: Sparrow Messenger PoC met with skepticism over bloat and fees
description: 
tags: services
image: 
---

dvd280[^1] recently proposed a new utility for Monero, as a censorship resistant private messaging platform[^2].

Today he announced[^3] Sparrow Messenger[^4], a proof-of-concept C++ *barebone module for enabling private communication through the Monero blockchain*:

    Alice and Bob want to communicate privately.
    Each of them has their own primary address.
    Both want to establish a private way to communicate.
    Each of them creates a secondary Monero address, and shares it only with the other.

> For every character the user sends, a transaction fee is claimed by the networks miners.[^5]

The community reacted with skepticism, pointing at several issues that might arise, mainly:

- blockchain bloat
- high fees
- no forward secrecy
- impractical for everyday use 


rbrunner7[^6] pointed out the recent Monero transaction flood incident[^7]:

> Somebody made nearly 400,000 transactions, paid around USD 1,000 for it, and produced around 600 additional MB in the blockchain. For basically a joke, as the analysis seems to hint at. Now thousands of people have to store that half gig on their harddisk as long as they use Monero, i.e. maybe decades. And everybody who syncs from scratch has to go through those 400,000 nonsense transactions.[^8]
 
HoboHaxor[^9] commented:

> I prefer my encrypted communications to be ephemeral, not last until the end of the universe.[^10]

AnarkioCrypto[^11] urged the community to defend the *status quo*:

> Please keep Monero as private, financially inclusive, KYC-free money. That's why it exists.[^12]

You can share your feedback for the dev in the discussion thread[^3] or by engaging with in the code repository[^4].

---

[^1]: https://github.com/dvd280
[^2]: https://libredd.it/r/Monero/comments/pqm1tq/monero_is_not_a_currency_at_all_its_a_censorship
[^3]: [https://libredd.it/r/Monero/comments/pvpgsr/i_created_a_c_module_for_encrypted_communication/](https://libredd.it/r/Monero/comments/pvpgsr/i_created_a_c_module_for_encrypted_communication/){:target="_blank"}{:rel="nofollow"}
[^4]: [https://github.com/dvd280/sparrow-messenger](https://github.com/dvd280/sparrow-messenger){:target="_blank"}{:rel="nofollow"}
[^5]: https://libredd.it/r/Monero/comments/pvpgsr/i_created_a_c_module_for_encrypted_communication/hebqr3o/?context=3
[^6]: https://libredd.it/user/rbrunner7
[^7]: https://libredd.it/r/Monero/comments/pvm634/fingerprinting_a_flood_forensic_statistical/
[^8]: https://libredd.it/r/Monero/comments/pvpgsr/i_created_a_c_module_for_encrypted_communication/hebqxp6/?context=3
[^9]: https://libredd.it/user/HoboHaxor
[^10]: https://libredd.it/r/Monero/comments/pqm1tq/monero_is_not_a_currency_at_all_its_a_censorship/hdc9szk/?context=3
[^11]: https://libredd.it/user/AnarkioCrypto
[^12]: https://libredd.it/r/Monero/comments/pqm1tq/monero_is_not_a_currency_at_all_its_a_censorship/hdd8rir/?context=3
