---
title: Plex + NZB + Raspberry PI
date: 2016-12-03 20:38:33
category:
- Home automation
tags:
- Plex
- NZB
- Raspberry PI
- NZBGet
- NewsHosting
- Usenet
- Sonarr
- Couch Potato
- TV
- Movies
- Automation
---
This is a guide to rolling out your own customizable alternative to a [Kodi Box](https://www.reddit.com/r/kodi/). By the end of this guide you will have a fully automated cross-platform media player, updated with all of your favorite tv shows and movies. My favorite part about this stack is once it is complete it requires little to no upkeep. Also I don't need to constantly be monitoring subreddits for when season 3 of [Rick and Morty](http://rickandmorty.wikia.com/wiki/Rick_and_Morty_Wiki) comes out, it will download the first episode as soon as it comes out and drop it on my [Plex](www.plex.tv) immediately. Enough hype, let's get started.

## Preface
We are going to be utilizing Usenet and NZBs to download the shows. If you are unsure about what these are, the legal ramifications, or the difference between this and torrenting, I suggest that you read up about on the [/r/usenet FAQ here](https://www.reddit.com/r/usenet/wiki/faq). Usenet is overall better than torrents for our purpose here because we will get better and more reliable download speeds and we will avoid bandwidth caps from our ISPs because we are not seeding any of our downloaded files.

## The Stack
So to achieve a fully automated entertainment downloader and displayer we are going to need to set up a few things:
1. A Usenet
