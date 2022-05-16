---
layout: post
category: story
title: Monero Observer self-hosted CLI Git server deployed
description: "Monero Observer's self-hosted terminal-based Git server has been deployed and is now accepting SSH connections to 'git.monero.observer' at port '23231'."
tags: [meta, guide]
image: 
date: 2022-05-14 22:00
---

Monero Observer's self-hosted terminal-based Git server has been deployed and is now accepting SSH connections to *git.monero.observer* at port *23231*.

The server hosts the open-source website code and content for the project. Read the licenses[^1] section for more info.

## Requirements

(1) To access the server (TUI) and browse the repository

- a terminal
- a SSH key pair (preferably *Ed25519* or *SHA-1 RSA*)

(2) To download the repository
 
- (1) & `git`

## Commands

- To generate a *Ed25519* SSH key pair run:

`ssh-keygen -o -a 75 -t ed25519`

- To access the TUI run:

`ssh git.monero.observer -p 23231`

- To clone the repository run:

`git clone ssh://git.monero.observer:23231/src`


That should covers the basics.

Thanks to git, ssh key pairs and `soft-serve`[^2], there is no need to touch browsers, *MS Github* or other proprietary/bloated platforms. Always remember that GitHub, GitLab et al != Git.

More guides on how to use git, ssh, terminals and email to collaborate cypherpunk-style will be available soon on Monero Observer.

Your questions, feedback and suggestions are always welcome @ [/about](/about#signature).

**-3RA**

---

[^1]: [/about#licenses](/about#licenses)
[^2]: https://github.com/charmbracelet/soft-serve
