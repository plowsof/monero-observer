---
layout: post
category: story
title: "Monero GUI v0.17.3.2 'Oxygen Orion' released with experimental support for P2Pool mining"
description: "The official Monero GUI v0.17.3.2 *Oxygen Orion* Point Release is out and it comes with experimental support for P2Pool mining and Ledger Nano S Plus."
tags: wallets
---

The official Monero GUI v0.17.3.2 *Oxygen Orion* Point Release[^1] is out and it comes with experimental support for P2Pool mining[^2] and Ledger Nano S Plus.

## Highlights

- Integrate experimental support for P2Pool mining (#3829)
- Warn against high fees during transaction creation (#3897)
- Add support for Ledger Nano S Plus
- Add support for reserve proof (#3828)
[..]

Note that this is the first GUI release with P2Pool support and bugs are expected, as the software is not well tested yet.

Support for P2Pool was previously added to the Monero CLI wallet in version 0.17.3.0[^3]. 

To view the complete list of changes, visit the Monero repository[^1] and compare changes with the previous version[^4].

The new binaries (CLI/GUI) can be found on the Downloads[^5] page on Getmonero.org.

## Contributors

- 22 contributors put out 76 commits containing 31625 new lines of code in `monero-gui`.

- 10 contributors put out 28 commits containing 2294 new lines of code in `monero`.

### GUI

```
selsta
luigi1111
rating89us
netrik182
devhyper
mj-xmr
jeffro256
reemuru
```

Special thanks goes to the translators: Miguel Medina, jaime diaz, Dynse Clyde Sacote, Robbie Monero, Gilberto F da Silva, Malek Atwiz, nanostos, ambercookie, Patix0331, Paul Janowitz, Trendyne, siptruk, tuknag, Marta Kozera.

### CLI

```		
luigi1111
Gingeropolous
woodser
jeffro256
hbs
moneromooo
reemuru
UkoeHB
erciccione
selsta
```

The latest release notes and downloads for both wallets are also included in selsta's Getmonero.org announcement posts[^6]'[^7].

Before installing anything you should check that the hashes of your files match those on the signed list, and that the signature on the list is valid[^8]. If you need help with the verification process, consult the Windows (beginner)[^9] and Linux/Mac/Win CLI (advanced)[^10] guides.

---

[^1]: [https://github.com/monero-project/monero-gui/releases/tag/v0.17.3.2](https://github.com/monero-project/monero-gui/releases/tag/v0.17.3.2){:target="_blank"}{:rel="nofollow"}
[^2]: https://github.com/monero-project/monero-gui/pull/3829
[^3]: [/monero-v0.17.3.0-oxygen-orion-point-release-p2pool-support/](/monero-v0.17.3.0-oxygen-orion-point-release-p2pool-support/)
[^4]: https://github.com/monero-project/monero-gui/compare/v0.17.3.1...v0.17.3.2
[^5]: [https://www.getmonero.org/downloads/](https://www.getmonero.org/downloads/){:target="_blank"}
[^6]: [https://www.getmonero.org/2022/04/29/monero-GUI-0.17.3.2-released.html](https://www.getmonero.org/2022/04/29/monero-GUI-0.17.3.2-released.html){:target="_blank"}
[^7]: [https://www.getmonero.org/2022/04/29/monero-0.17.3.2-released.html](https://www.getmonero.org/2022/04/29/monero-0.17.3.2-released.html){:target="_blank"}
[^8]: https://www.getmonero.org/downloads/hashes.txt
[^9]: https://www.getmonero.org/resources/user-guides/verification-windows-beginner.html
[^10]: https://www.getmonero.org/resources/user-guides/verification-allos-advanced.html
