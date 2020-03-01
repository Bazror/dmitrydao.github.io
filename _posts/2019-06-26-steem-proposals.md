---
layout: post
title: "Steem Proposals UI Launch"
categories: steem
author: "Dmitry Baimuratov"
---

Hey guys. Over the last two months, I was visiting different countries to see the differences in cultures, technologies, and innovations. It was a great time for me to rethink my game and to understand what is really important in this life. I figured that I’m a lot better at pushing small projects, rather than working on something big.

When I was in Chiang Mai, Thailand I set myself a goal to finish what I started back in Bali – Steem proposals interface. Even though the project was almost complete, I wasn’t fully satisfied with what I had. The interface was good but primitive and the technology I used didn’t allow me to have a structured and readable code.

This one caused me to learn a brand-new framework (Vuejs) and create [this project](https://steemproposals.com/) from scratch. Honestly, it was the best thing I’ve ever done because using state management techniques (Vuex) my code became extremely clean and easy to manage in the long run.

## Launching the first Steem Proposal System UI

That leads us towards the project itself. Correct me if I’m wrong but outside of Steemit Inc, this can be the [first portal](https://steemproposals.com/) that introduces a visual representation of the SPS system. I’m extremely excited to bring it to you guys because I believe it’s very important to have an appealing way to browse through projects that can potentially help Steem to become a top blockchain in terms of usage, as well as STEEM to become a top coin in terms of market share.

I had three iterations of this particular project but I think I will stop with this one and just add more features over time. I also have three main concepts that I would like to outline:

A. **Mobile-driven**. Since our phone is the main device we’re spending the most amount of time on, I did my best to make sure that you get a pleasant experience of looking through the latest proposals when you feel like doing so. It’s kind of intuitive that people grab their phone first when they need to get some info on a spot, rather than open up their laptop. However, I still see projects missing this point and I don’t really understand why.

B. **Data-driven**. Traditionally an interface like this would have a simple list of proposals and that’s basically it. I decided to go further and add some extra data that might be useful to make your voting decision. Thus, each worker has its own page that shows the reputation, the number of posts and followers, as well as all of the projects one was working on or is currently performing. There’s also a separate page for all of the workers who submitted at least one proposal which can be useful when we’ll have more people asking for funds.

![mock2.png](https://cdn.steemitimages.com/DQmS9cCcKkLPXzr5drJK2igjCJ54nxKUC4N5Q2xRmVoZYm1/mock2.png)

C. **Community-driven**. Since this is a project for a Steem community, I would like to receive as much input and feedback as possible. In this way, we can gradually make what we really need together. So please, don’t be shy, pour everything you like and don’t like. We’ll get there.

## Things to keep in mind
- [steemproposals.com](https://steemproposals.com/) is only one of the interfaces that anybody can create to display a list of Steem proposals.
- I plan on open-sourcing the code if I see a demand from other developers to implement the voting functionality within this portal directly.
- Originally the data from queried from mock proposals, now it's fetched from Steemit testnet.
- FAQ is currently incomplete. Please, let me know what kind of questions do you think people will ask over and over again. We can fill this one together.
- `Create proposal` page is not accessible at the moment because you can only create a proposal from the CLI wallet. I will add detailed instructions on how to submit a proposal through CLI as soon as SPS goes live. I will try to do that for each wallet that implements SPS functionality.
- Total budget (`funds_in_funding_account`) is currently set to $30,000. Eventually, the amount will be fetched from the SteemDAO account.
- Daily budget is calculated using the formula [mentioned](https://steemit.com/blocktrades/@blocktrades/proposing-a-worker-proposal-system-for-steem) by @blocktrades: `daily_budget_limit = funds_in_funding_account/100 + daily_worker_inflation`. However, the way `daily_worker_inflation` is calculated can be changed, so it will adjust as soon as it becomes clearer. At the moment daily_inflation is 50% of the `funds_in_funding_account` which is $15,000.

Thanks a lot for going through this, I really appreciate your help and support. I believe SPS will create a healthier development and marketing ecosystem for Steem so let’s do it together.

P.S. With the latest update you can check the proposals from Steemit Testnet.

