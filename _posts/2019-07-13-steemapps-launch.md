---
layout: post
title: "Steem Apps Explorer Launch"
categories: steem
author: "Dmitry Baimuratov"
---

Since my last launch of [Steem Proposals](https://steemproposals.com) I figured that I love building products for communities, not companies. I was never a fan of working in an office simply because of the same routine and environment. But when you have a chance to choose your work and life location, you become more excited and energized, which leads towards more creative and awesome things.

Today I’m announcing my third product which is a Steem Apps Explorer. With a rising demand for apps and dapps that leverage Steem blockchain it is simply impossible to ignore the fact that we need a better way of presenting data that is coming through this powerful blockchain. That’s why I decided to make something simple, yet elegant for you to browse through recent or targeted transactions within various apps a Steem blockchain has to offer.

## Why another explorer?

You might wonder why to create yet another explorer when there a few already? Simple, alternative. The existing explorers (steemd, steemdb, steemblockexplorer) haven’t updated their UI since the first launch and if you look at their target audience, it’s mostly nerds and tech people. I want to create something that anybody can use and understand without going deep in research in what is `required_auths` is. 

Moreover, I’m not creating this to compete but to give you an option to choose from when you need to check the details about certain transactions. Some people love lists, the others prefer cards and there are table addicts so there’s room to expand for sure.

Besides, at the moment you just simply can’t find transactions that belong to a certain application built on Steem, it’s not the main focus of current developers since there’s a huge incentive deficit for any developer. You can do an app but it takes more time and effort to maintain it without any funding whatsoever.

Lastly, my plan is to expand this explorer to SMTs, tribes, and communities that you all are excited about.

## What is the official link?

If you're really impatient, you can just go straight to [steemappsdb.com](https://steemappsdb.com)

## An overview of Steem Apps Explorer
So here’s a brief overview of explorer. 

![1.png](https://cdn.steemitimages.com/DQmUXCiK43hEHUE5NLNvc3MUZVeWPjhxMGYQdqnyWK4qZKj/1.png)
 
First things foremost, I didn’t add all of the available apps on the network because this is simply impossible due to the fact that I don’t know each of their `custom_json` operations. I will add them gradually as I receive more requests and approach apps developers by myself. At the moment the website supports [Steemit](https://steemit.com), @steemmonsters, [Steem Engine](https://steem-engine.com) and @nextcolony apps since they consume the most amount of transactions.

While it would be great to search using a transaction id, I haven’t found a way to do so using Steemit condenser API (the current functionality is simply deprecated). However, this is something I’m curious and need on my own, so I’ll do my best to make it happen at some point. Therefore, you can search transactions by a block id which should be enough at this point. I also want to add a search by account name which will be so much more fun to implement so stay tuned.

![](https://cdn.steemitimages.com/DQmf8tWHNt1nLVvscdaRMU68nNQznVuaaW4dmDTw7DBWJqk/image.png)

By the way, all of the data loads only when you make a change to the block id which means it doesn’t make an extra API call when you switch from one app to another. This is very handy and prevents redundant operations that can be done on a client-side. Don’t thank me, thank Vuex for this one.

Sometimes you might encounter `performed an unknown` or `performed operation_name` operation which simply means I wasn’t aware of its existence. If you find such things, just ping me and I’ll add it.

P.S. I's a fully mobile supported since this is where we live in right now in any case.

## How do I add new apps?

Currently, my approach is simple as it gets, I use `custom_json` for determining which app does this transaction belong to. It’s a straightforward model but it seems to be working cause most of the apps use it as a standard. I will consider adding account addresses to monitor bots and other apps that rely on exchanging assets only so expect a bot section soon because it is heavily, unfortunately.

## How to add your app?

In order for me to add your app here, just simply provide me with your `custom_json` you’re using for your operations. If you don’t use them, then give me some alternative on how I can track your app. I would really appreciate support and collaboration here because I see it as something that can help lots of people. Let me know what is important for you and your customers so that I can present it in a simpler and sophisticated visual form.  

If you have any question, feel free to message me at [Discord Group](https://discord.gg/eXxA5BN).