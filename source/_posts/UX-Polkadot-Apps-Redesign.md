---
title: UX proposal for Polkadot Apps
date: 2019-08-11 13:57:28
categories: portfolio
tags:
  - portfolio
cover_image: /images/polkadot-cover.png
---

<p style="color:#aaa;">Parity | Year: 2019</p>


### Overview
Recently, I started to pay attention to blockchain technology and decentralized applications. I am really fascinated by the idea of decentralized web and I believe it’s the trend of the future web. In July, I was lucky to have an UX Developer job interview with [Parity Technologies](https://www.parity.io/). In the hiring process, they asked me to take a look at [Polkadot Apps](https://polkadot.js.org/apps) and provide a short writeup of my thoughts on improvements of one of the views that could be made from a UX perspective​.​ Polkadot Apps is a basic Polkadot/Substrate UI for interacting with a node. It is the main user-facing application, allowing access to all features available on Polkadot/Substrate chains. Although I didn't get the job in the end, I still learned a lot from the process and decided to summarize the UX tasks I did here.

---

### Polkadot Apps Redesign - App-Explorer
First, I took a close look at page app-explorer on Polkadot Apps. **It’s the page showing recent blocks and events on the chain.** One can also click on a block to see more detail of it, including parentHash, timestamps,etc... From user experience perspective, I wrote down several points that could be improved. At the meantime, I cloned the whole project from https://github.com/polkadot-js/apps and tried to code up the UX issues I proposed.

#### Problems and Design Proposals:
1. **Responsive issue**
First of all, when I look at page app-explorer, the experience on mobile isn’t friendly. Blocks are cut off and can’t even scroll horizontally to view. So I fixed the responsive layout and emphasized each block with shadow and card-like design as well as reduced the information showing on the card to provide a clear impression at first sight.

<img src="https://drive.google.com/uc?export=view&id=1gIZoQkhpswzkz2bw0Wi8v3psi85D48sz" width="100%" height="auto"/>

2. **Block updating is not obvious**
The updating of the blocks isn’t obvious enough because block number is updating only in one digit and hash is just a string of garbled code which is hard to notice the difference immediately. Currently, when new block was added into the list, it just popped up causing users have to pay more attention on what’s going on the page. So I decided to add a fade in effect on the newest block and push down the whole list. These little animations seem to be small but they make the browsing experience more delightful and effortless.

<div style="text-align:center;">
<video id="video"  preload="auto" autoplay loop>
<source id="mp4" src="/images/Polkadot-1-1.mp4" type="video/mp4">
</video>
<p style="font-weight:bold;font-size:18px;color:black">Current Version</p>
</div>

<div style="text-align:center;margin-bottom:10px;">
<video id="video"  preload="auto" autoplay loop>
<source id="mp4" src="/images/Polkadot-1.mp4" type="video/mp4">
</video>
<p style="font-weight:bold;font-size:18px;color:black">Updated Version</p>
</div>

3. **Recent blocks showing 16 blocks is too much**
I found out currently it’s showing 16 blocks in recent block column. If there’s no specific reason for this number, I think would be better to only show no more than 7 blocks because the capacity of human beings’ working memory is rather small, our attention is considerably selective and it makes no sense to show that much in recent blocks. In addition to that, 16 blocks will overflow the fold causing users have to scroll down and it’s also an unnecessary behavior.

<img src="https://drive.google.com/uc?export=view&id=1CmzEChDUjdnTwcyY2cvLsgPcl5lN5EBM" width="100%" height="auto"/>

4. **Placing block details on tab is not suitable**
Block details page is now placing on the tab with same hierarchy as chain info and node info, which is a bit weird. When users click on a block, it shows the details of that block, so from information architecture perspective, block details should be another level deeper than chain info. For this case, since I decided to make each block as card-like design, I would suggest to leverage the power of card design. Card is a flexible container that can add different animations to expand it to reveal more content.

<div style="text-align:center;margin-bottom:40px;">
<video id="video"  preload="auto" autoplay loop>
<source id="mp4" src="/images/Polkadot-2.mp4" type="video/mp4">
</video>
</div>

---

### Polkadot Apps Redesign - Staking
Besides page explorer, I also took a look at staking page on Polkadot Apps. **Staking is an important feature for one to get involved in Polkadot network as either a validator (running a node that helps secure the network), or a nominator (adding funds to help secure the network).**

#### Research and Insights:
There are two main users(roles) on staking page: validator and nominator. To start off, I asked myself, what really matters to users? Through putting myself into their shoes, I can better imagine UX issues they might encountered.

1. **As a nominator, I want to ..., so I can...**
  * As a nominator, I want to know which validators are deemed trustworthy, so I can stake fund to them. (What is trustworthy? Having the most nominators? Having the best reputation without any warning? Having the most DOTs?)
  **Insight: To achieve finding which validator is trustworthy, one might need "Filter + Sort".**

  * As a nominator, I want to know which validators have less nominators but with good reputation, so I can stake fund to them and make better profit.
  **Insight: To achieve better profit, one might need "Multi-filter" to find those validators with less nominators but with good reputation.**

2. **As a validator, I want to ..., so I can...**
  * As a validator, I want to know my ranking among all validators, so I know if I have a chance to get rewards.
  **Insight: To achieve knowing how likely to get rewards, one night need "Stakeholding Sort"**

From the brief research above, I found that adding "Filter" which supporting muliple filtering and sorting to staking page is necessary. Currently on Polkadot Apps, there is a filter on the right corner of staking page. But it only enables single selection. Also the position of the filter is not obvious enough.

<img src="https://drive.google.com/uc?export=view&id=1MBSua85Y7PDOZeGWYcKIYYQf-60ra5XD" style="margin-bottom: 40px" width="100%" height="auto"/>

#### Design Proposals:
I redesigned the staking page by changing the placement of the filter. Enable multi selection on filter. Also it's responsive and mobile-friendly.

<div style="display:flex;align-items:center;justify-content:space-between;flex-wrap:wrap;margin-bottom:40px;">
<img src="https://drive.google.com/uc?export=view&id=1iI3nHa5aKfYpAP45wx6Jd6tVmnz6Yyoh" width="213px" height="auto"/>
<img src="https://drive.google.com/uc?export=view&id=1udcKiGbOyhe6qVtrIpofLxqoBgJXPZ0l" width="213px" height="auto"/>
<img src="https://drive.google.com/uc?export=view&id=1keFRo_5FjinRwrJZsHqI9Zby-ph7c65B" width="213px" height="auto"/>
</div>

I also coded up my design proposal in the end:
<div style="text-align:center;margin-bottom:40px;">
<video id="video" width="100%" height="auto" preload="auto" autoplay loop>
<source id="mp4" src="/images/Polkadot-3.mp4" type="video/mp4">
</video>
</div>

### Conclusion
I enjoyed very much researching and solving UX issues of Polkadot Apps while taking the job interview with Parity. I think I already tried my best within the limited time and had learned a bunch of blockchain knowledge during the process. Blockchain technology is gradually changing our world with its power of enabling trust among decentralized nodes. However, this area is still relatively new to normal UI/UX designers. I know it definitely needs more UI/UX practitioners jumping in because no matter how technologies change, we always are dealing with people. And I have a lot of passion being a pioneer to explore more possibilities in this area.

