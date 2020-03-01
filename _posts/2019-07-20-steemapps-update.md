---
layout: post
title: "Steem Apps Explorer Update"
categories: steem
author: "Dmitry Baimuratov"
---

Hey! Just pushed a new update of [Steem Apps Explorer](https://steemappsdb.com). This one was quite a challenge for me because turned out people use custom_json in whatever way they want which causes occasional issues to arise. I was fighting one bug after another but now it seems like I handled most of them.

Here's a quick screen of a new version:

![](https://cdn.steemitimages.com/DQmYiGF4QFzbsVGPvfztY362gpQHDuKpuP9HEc5SuRednf6/image.png)

Anyways, this release includes the following:
- Support of over 30 apps. I decided not to add all of the available apps from SteemApps.com simply because a lot of them have no significant volume whatsoever.
- A list of all transactions. This one I didn’t implement before because of poor code management. 
- A new tabs interface for apps. The coolest part is that you can use left/right or up/down buttons on your keyboard to navigate through the apps, instead of manually clicking on them.
- Previous/Next buttons. This one somebody suggested in the comments, adds a utility when you want to check what type of transactions most of the blocks consist of.
- About and Support page that leads to a discord group in case you want to chat or have some questions.
- 6 metrics: custom_json, transfers, votes, replies/comments/posts, json_metadata (both apps and tags), Steem-engine tokens
- A separate tab for Tribes. This one became a major growth factor for Steem on-boarding and currently brings loads of attention, traffic, and usage. I’m not that familiar with tribes, so I would highly appreciate if somebody can guide me through which are a must to add here. I already included such Steem-engine tokens as tribes with respective tags and accounts - `'PAL', 'NEOXAG', 'CCC', 'LEO', 'GG', 'SCT', 'STEM', 'NATRL', 'SONIC', 'AAA', 'ACTNEARN', 'ASS', 'ATTDUMMY', 'BATTLE', 'BLQ', 'BPC', 'CTP', 'DOLPHIN', 'ENG', 'INT', 'IV', 'JAHM', 'LIFESTYLE', 'LIV', 'MARLIANS', 'MOT', 'NGA', 'RHB', 'SPACO', 'SPORTS', 'TMT', 'TUNES', 'UFM', 'WEED', 'ZZAN', 'BEER'`. But I’m not sure this is the whole list since I’ve seen hundreds of tokens. Maybe I should add all of them? Your thoughts?

For those who want to be listed on explorer, here’s a format that I use in order to track any particular app:
```
{ 
        text: 'Actifit',
        value: 'actifit',
        customJson: [],
        accounts: ['actifit', 'actifit.pay', 'actifit.funds', 'actifit.signup'],
        metadataTags: ['actifit', 'afit'],
        metadataAppNames: ['actifit'],
        scotTokens: ['AFIT', 'AFITX'],
        image: 'https://steemitimages.com/u/actifit/avatar'
}
```
