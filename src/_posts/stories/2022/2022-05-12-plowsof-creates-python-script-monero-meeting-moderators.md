---
layout: post
category: story
title: "plowsof creates Python script for Monero meeting moderators"
description: "plowsof has created a small Python script that aims to help Monero meeting moderators  auto post logs to the correct '-meta' issue on Github."
tags: services
date: 2022-05-12 20:00
---

plowsof[^1] has created a small Python script[^2] that aims to help Monero meeting moderators  auto post logs to the correct *-meta*[^3] issue on Github:

> for meeting moderators who are tired of copy and pasting logs -> posting them to the monero meta issue and then closing the issue.[^4]

The script uses the *PyGithub*[^5] library and requires a user's git token[^6] with public repository access.

To learn how to configure and run the script, consult plowsof's *post-libera-meeting-logs* repository README file[^7]. 

---

[^1]: https://github.com/plowsof
[^2]: [https://github.com/plowsof/post-libera-meeting-logs/blob/main/post_logs.py](https://github.com/plowsof/post-libera-meeting-logs/blob/main/post_logs.py){:target="_blank"}{:rel="nofollow"}
[^3]: https://github.com/monero-project/meta/issues
[^4]: https://libera.monerologs.net/monero-community/20220512#c93943
[^5]: https://github.com/PyGithub/PyGithub
[^6]: https://github.com/settings/tokens
[^7]: [https://github.com/plowsof/post-libera-meeting-logs](https://github.com/plowsof/post-libera-meeting-logs){:target="_blank"}{:rel="nofollow"}
