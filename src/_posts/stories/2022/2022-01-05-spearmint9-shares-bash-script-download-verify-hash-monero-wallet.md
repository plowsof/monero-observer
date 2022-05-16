---
layout: post
category: story
title: Spearmint9 shares bash script that downloads and verifies hash of Monero GUI wallet latest version
description: "Spearmint9 has shared a simple tool, a bash script, that downloads and verifies the hash of the latest version of Monero GUI wallet."
tags: [wallets, services]
image: 
---

Spearmint9[^1] has shared[^2] a simple tool, a bash script[^3], that downloads and verifies the hash of the latest version of Monero GUI wallet[^4]:

> This script downloads and verifies the hash of the latest version, if successful, the download is then extracted at the specified destination.

Note that the script does **not** download, verify and import the GPG signing key[^5]. It is recommended to do that manually by following the guides on Getmonero.org[^6]'[^7]. There's also a Monero Observer guide available for the CLI wallet[^8].

Make sure to inspect the latest version of the code[^9] before executing the script. You can post your feedback on Github[^3] and Reddit[^2].

---

[^1]: https://github.com/Spearmint9
[^2]: https://libredd.it/rw5o7p
[^3]: [https://github.com/Spearmint9/monero-linux-scripts](https://github.com/Spearmint9/monero-linux-scripts){:target="_blank"}{:rel="nofollow"}
[^4]: https://www.getmonero.org/downloads/
[^5]: https://github.com/monero-project/monero/blob/master/utils/gpg_keys/binaryfate.asc
[^6]: https://www.getmonero.org/resources/user-guides/verification-windows-beginner.html
[^7]: https://www.getmonero.org/resources/user-guides/verification-allos-advanced.html
[^8]: [/verify-install-update-monero-cli-wallet-linux-guide/](/verify-install-update-monero-cli-wallet-linux-guide/)
[^9]: https://github.com/Spearmint9/monero-linux-scripts/blob/master/download-and-verify-latest.bash
