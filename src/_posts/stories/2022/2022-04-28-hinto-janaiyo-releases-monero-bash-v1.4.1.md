---
layout: post
category: story
title: hinto-janaiyo releases monero-bash v1.4.1
description: "hinto-janaiyo has released v1.4.1 of Monero Bash wrapper for Linux, 'monero-bash'."
tags: mining
image: 
date: 2022-04-28 20:00
---

hinto-janaiyo[^1] has released v1.4.1[^2] of Monero Bash wrapper for Linux, *monero-bash*[^3].

## Changes

- gpg verification is now always on when installing/upgrading packages
- `gpg toggle` & `gpg import` deprecated
- `update` bug fix
- wallet files (key images, signed transactions) are now created in `~/.monero-bash`
- `xmrig` hugepage = 1280, the rest are 1024

The sources, SHA256SUM and .asc files can be found on Github[^2]. Always verify before using.

To learn more about the project, read the associated CCS proposal[^4] and my previous report[^5].

---

[^1]: https://github.com/hinto-janaiyo
[^2]: [https://github.com/hinto-janaiyo/monero-bash/releases/tag/v1.4.1](https://github.com/hinto-janaiyo/monero-bash/releases/tag/v1.4.1){:target="_blank"}
[^3]: https://github.com/hinto-janaiyo/monero-bash
[^4]: https://ccs.getmonero.org/proposals/monero-bash.html
[^5]: [/hinto-janaiyo-submits-ccs-proposal-monero-bash/](/hinto-janaiyo-submits-ccs-proposal-monero-bash/)
