---
layout: post
category: story
title: Read Monero Observer inside your terminal using Newsboat RSS feed client
description: Read Monero Observer inside your terminal using Newsboat RSS feed client
tags: guides
image: newsboat.png
---

## Motivation

In an effort to increase profits, website owners have started using social media, newsletters, apps and trackers. The main casualty of this process is the user's privacy.

There is a way to stop trading privacy for content/notifications and break that dependency on browsers, emails and all that bloat: **RSS**.

*Really Simple Syndication*[^1] has been around for a long time. It was and still is arguably one of the best way to consume content. You can use RSS to stay up to date with pretty much any website: blogs, video channels, git repos, tweets, posts and news sites.

**Newsboat**[^2] is an open-source RSS feed reader/client for your terminal. It's lightweight, extensible and has terminal notifications.

## Assumptions

- you are running a Unix/Unix-like system (GNU/Linux, FreeBSD or macOS)

## Installation

There are several ways to install Newsboat:

### A. Using a pre-built binary for your OS[^3] (easy, recommended)

In Debian 10 for instance, you can run `sudo apt install newsboat`.

Note that this might install an outdated/legacy version of the application. 

There's a non-exclusive list[^4] you can refer to. Search for the Newsboat version that is maintained for your OS.

### B. From the Snap Store[^5] (easy, not recommended)

If you want to use Snap, just run: `sudo snap install newsboat`.

### C. From source[^6] (advanced, most secure, latest version)

You will get the most up-do-date source code, regardless of what is packaged in your OS, if you can build Newsboat from source.

After you download the source code, install dependencies and compile, you can finally install Newsboat.

## Configuration

Once installation is completed, you can simply type `newsboat` in your terminal to start it.

It is expected to get an error message similar to this one:

`Error: no URLs configured. Please fill the file /home/ak/.newsboat/urls with RSS feed URLs or import an OPML file.`

Let's do just that.

- `nano .newsboat/urls`
*(opens the urls file in nano text editor)*

Paste in the Monero Observer RSS feed urls, one per line:

```
https://monero.observer/feed.xml
https://monero.observer/feed-ta.xml
https://monero.observer/feed-blitz.xml
```
Save and exit (CTRL+X if you used `nano` to edit the file).

This is the minimum configuration needed to run Newsboat. You can tweak it and make it your own by consulting Newsboat's documentation[^7].

## Usage

As soon as you have some feeds in your `urls` file, run `newsboat` again and press `R` to refresh all feeds.

Navigate using your arrow keys and by pressing the *Enter* key to select a feed; press it again to read a specific article. 

Pressing `Q` brings you back to the previous screen. Exmaple: if you are on the article list of a feed and press it once, you go back to the feeds list; pressing it twice quits Newsboat.

This is all basic usage and should help you get around, but you can bind your own keys and do lots of fancy things with Newsboat. Everything is in the docs.

## Features

Newsboat is not lacking in features. Here are a few:

- Newsboat automatically caches the article that it downloads, so if an article is removed from the RSS feed by the website's owner, you can still read it.

- You can search by pressing `/` and entering your query. Newsboat will search both titles and content. If you wish to search every article of every feed, make sure you are on the all feeds screen, otherwise it will only search inside a specific feed.

To add terminal notifications, just edit the config file:

- `nano ./newsboat/config`
*(opens the config file in nano text editor)*

Paste in the following instructions:

```
auto-reload yes
reload-time 5
reload-threads 500
notify-screen yes
notify-beep yes
notify-xterm yes
notify-format "Newsboat: %n new/%f feeds"
```

Save and exit.

Newsboat will auto-reload all feeds every 5 minutes and notify the terminal of new activity by changing the window title: *Newsboat: 21 new/3 feeds*. Change the values as you see fit.

## Privacy

Use Newsboat in Qubes/Whonix/Tails, or torify the connection by running one of the following commands:

- `torsocks newsboat`
- `torify newsboat`
- `proxychains4 newsboat`

## Notes

To further explore Newsboat, I suggest you read the docs and search the net. I will also try to assist, if you email me.

Luke Smith's videos[^8] on RSS & Newsboat are excellent guides. You can also subscribe to his feed by adding `https://lukesmith.xyz/rss.xml` to your `.newsboat/urls` file.

There are lots of RSS readers out there, you just have to find the one you like best. For people that actually *live* in the terminal, I'm sure Newsboat is #1.

## Feedback

How are you reading Monero Observer? I'm curious.

If you find these guides helpful, I will create more.

Contact details @ [/about](/about).

**-3RA**
 

---

[^1]: https://en.wikipedia.org/wiki/RSS
[^2]: https://newsboat.org
[^3]: https://newsboat.org/releases/2.25/docs/newsboat.html#_pre_built_binaries
[^4]: [https://repology.org/project/newsboat/versions](){:target="_blank"}{:rel="nofollow"}
[^5]: https://snapcraft.io/docs/installing-snapd
[^6]: https://newsboat.org/releases/2.25/docs/newsboat.html#_from_source
[^7]: [https://newsboat.org/releases/2.25/docs/newsboat.html#_newsboat_configuration_commands](https://newsboat.org/releases/2.25/docs/newsboat.html#_newsboat_configuration_commands){:target="_blank"}
[^8]: [https://videos.lukesmith.xyz/search?search=rss&searchTarget=local](https://videos.lukesmith.xyz/search?search=rss&searchTarget=local){:target="_blank"}


