---
layout: post
category: story
title: The Farcaster Project releases initial version 0.1.0 of Farcaster Node
description: "The Farcaster Project has released the initial version (0.1.0) of the Farcaster cross-chain atomic swap node."
tags: services
image: 
date: 2021-12-10 20:00
---

The Farcaster Project[^1] has released the initial version (0.1.0)[^2] of the Farcaster cross-chain atomic swap node[^3]:

> The Farcaster Node is a collection of microservices for running cross-chain atomic swaps. Currently the node is focused on Bitcoin-Monero atomic swaps, but is designed to be flexible and integrate new crypto-pairs in the future. 

Note that the tech is still experimental. Do not try using the software on mainnet or with real money.

### Added in v0.1.0

    Bitcoin SegWit v0 support as arbitrating chain
    Monero support as accordant chain
    Bitcoin and Monero syncers
    Swap daemon to manage single swap execution
    Peer daemon to manage p2p connection during swaps
    Farcaster daemon to orchestrate the micro-services
    Swap cli to control farcasterd and other services

To get involved with the project, join *#monero-swap* on IRC/Libera.

---

[^1]: https://github.com/farcaster-project
[^2]: [https://github.com/farcaster-project/farcaster-node/releases/tag/v0.1.0](https://github.com/farcaster-project/farcaster-node/releases/tag/v0.1.0){:target="_blank"}{:rel="nofollow"}
[^3]: https://github.com/farcaster-project/farcaster-node


