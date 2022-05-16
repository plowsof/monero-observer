---
layout: post
category: story
title: Beta-9 is the last Feather wallet release before 1.0.0
description: Beta-9 is the last Feather wallet release before 1.0.0. 
tags: wallets
image: 
---

The newest Feather[^1] wallet release, Beta-9[^2], has been available on the website for a few days now.

Some users have been patiently waiting for tobtoht[^3], the the lead dev, to confirm the update by adding the Beta-9 tag on Feather's Gitea repository[^4], before using this new version. 

MoneroArbo[^5] commented:

> Release seems signed by the correct key but there's no beta-9 tag on github, the auto updater isn't notifying me, and updates are normally posted here by /u/tobtoht 

> Seems weird. I'm gonna wait.

Feather will go out of Beta with the next release, according to tobtoht:

> This is the last Beta release before 1.0.0.[^6]

> This release has been available from the website and via the auto updater on AppImage builds for a few days, my apologies for the delayed announcement.

It is recommended to update to Beta-9, as it uses the latest Monero v0.17.2.3 which fixes the *decoy selection bug*[^7].

A GPG-signed list of the hashes[^8] can be found on the website. The signing key[^9] is in the Git repo.

Don't trust. Verify.

---

[^1]: https://featherwallet.org/
[^2]: [http://featherdvtpi7ckdbkb2yxjfwx3oyvr3xjz3oo4rszylfzjdg6pbm3id.onion/download/](http://featherdvtpi7ckdbkb2yxjfwx3oyvr3xjz3oo4rszylfzjdg6pbm3id.onion/download/){:target="_blank"} (onion)
[^3]: https://git.featherwallet.org/tobtoht
[^4]: https://git.featherwallet.org/feather/feather/tags
[^5]: https://libredd.it/user/MoneroArbo
[^6]: https://libredd.it/r/FeatherWallet/comments/pu23cp/feather_beta9_released_decoy_selection_bug_fixed/
[^7]: https://github.com/monero-project/monero/pull/7822
[^8]: http://featherdvtpi7ckdbkb2yxjfwx3oyvr3xjz3oo4rszylfzjdg6pbm3id.onion/files/releases/hashes-beta-9.txt (onion)
[^9]: https://git.featherwallet.org/feather/feather/src/branch/master/utils/pubkeys/featherwallet.asc
