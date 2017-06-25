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

### Preface
We are going to be utilizing Usenet and NZBs to download the shows. If you are unsure about what these are, the legal ramifications, or the difference between this and torrenting, I suggest that you read up about on the [/r/usenet FAQ here](https://www.reddit.com/r/usenet/wiki/faq). Usenet is overall better than torrents for our purpose here because we will get better and more reliable download speeds and we will avoid bandwidth caps from our ISPs because we are not seeding any of our downloaded files.

### Software Stack
So to achieve a fully automated entertainment downloader and displayer we are going to need to set up a few things:
```
Total Cost: $110/year
```

1. [Usenet provider:][Usenet] I use [NewsHosting][NewsHosting]
2. [Usenet index:][Indexers] I use [DOGnzb][DOGnzb] and [NZBcat](https://nzb.cat/). *Note* You can find both free and paid indexers, obviously the paid ones will be more reliable. You can stack as many indexers as your heart desires to greater your chance of finding more obscure files.
3. [Usenet downloader:][Downloaders] I'm going to explain how to set up [NZBGet][NZBGet] here. No reason why I am using it over [Sabnzbd][Sabnzbd] just what I started with first.
4. Schedulers: [Sonarr][Sonarr] to track and request tv shows. [CouchPotato][CouchPotato] to track and request movies. *Note* [Headphones](https://github.com/rembo10/headphones) does the same but for music, but I haven't set it up yet.
4. [Plex:][Plex] For watching on computer, xbox, playstation, phone, etc.

### Hardware
You could avoid buying these by running the above on an old laptop or free server you have. I chose to dedicate hardware:
```
Total Cost: $150
```
1. [Raspberry PI 3: ][RaspberryPI3] To run the NZBGet + Sonarr + Plex. I recommend buying two of these and running NZBGet + Sonarr, and Plex separately.
2. Hard drive if you're more ephemeral with your content. Cloud storage if you're a hoarder.

### 0. Set up PIs (Skip this step if you're already set up on a computer)
First off you are going to need to set up your Raspberry PI with NOOBS. You can find a very [intuitive guide here.][NOOBSGuide]
### 1. Set up the [Usenet][Usenet] Provider
```
Usenet is a worldwide distributed Internet discussion system. It was developed from the general purpose UUCP architecture of the same name.
```
[Usenet][Usenet] does cost money, however it is basically as if you are paying for your mirror of the internet. You can stack Usenet to get even more reliable files but I never have any trouble finding shows or movies. [Here is a list of Usenet Providers][Providers]. I use [NewsHosting][NewsHosting] which costs $10 a month.

### 2. Connect Indexers

### 3. Configure Downloaders

### 4. Configure Schedulers

### 5. Connect Plex Server





[Usenet]: https://www.reddit.com/r/usenet/wiki/faq#wiki_what_is_usenet.3F
[Providers]: https://www.reddit.com/r/usenet/wiki/faq#wiki_providers
[NewsHosting]: https://www.newshosting.com/
[Indexers]: https://www.reddit.com/r/usenet/wiki/indexers
[DOGnzb]: http://www.dereferer.org/?https://dognzb.cr
[Downloaders]: https://www.reddit.com/r/usenet/wiki/faq#wiki_software_and_downloading
[Sabnzbd]: https://sabnzbd.org/
[Sonarr]: https://sonarr.tv/
[NZBGet]: http://nzbget.net/
[CouchPotato]: https://couchpota.to/
[RaspberryPI3]: https://www.raspberrypi.org/products/raspberry-pi-3-model-b/
[Plex]: https://www.plex.tv/
[NOOBSGuide]: https://www.raspberrypi.org/learning/noobs-install/
