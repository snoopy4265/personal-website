---
title: 2019 Berlin Blockchain Week（上）
date: 2019-08-20 13:37:47
categories: blog
tags:
  - blog
  - tutorial
cover_image: /images/BBW.png
---
柏林受益於本身高度自由開放且反資本主義的城市氛圍，是發展去中心化區塊鏈的溫床，在今年為期一週的Berlin Blockchain Week(BBW)裡，我報名參加了幾場活動，活動中我主要著重於了解Web3和Dapps有關UI/UX的探討，並整理了一些自己的Note和Takeaway。

<br/>
## How Web3 will be better than Web2?
> We haven’t seen a financial system that defines culture. But again, before facebook, we haven't seen a social media that defines culture.
如果說Web2.0是以社群和內容為王道，那Web3.0就是以去中心化、信任和隱私為王道，其實Web2.0和Web3.0並沒有太大的不同，許多Web3.0的應用程式仍要借鏡Web2.0的使用習慣，改變是一點一滴發生，而非一下強迫轉移。

![#buildbetter](/images/BBW-1.jpg)

有關Onboarding的UX issues仍然是Web3的熱門話題，比起提出解決辦法或提出可以遵循的UX Guidelines，我感覺更多的還是丟出問題到這個未解領域。例如How do we convey users in a meaningful way to use web3 applications? Who should responsible for the complexity, developers or users?

<br/>
## Problems we're facing in Web3 and Dapps:
Web3主張去中心化、主張不需透過第三方信任交易、主張保有個資隱私，但對一般的使用者來說，他們其實並不在乎去不去中心化，他們只在乎這個東西好不好用，或是能否從中獲利，然而現在整個Web3生態系，都只是讓使用的門檻越來越高，令人望之卻步。
從幾個面向拆解使用者在使用Dapps時可能遭遇的問題：
1. **Onboarding:** 超難onboard，為何要叫我換Web3 Browser？我要持有tocken才能用這個Dapp嗎？沒有tocken就不能用嗎？
2. **Tocken exposure:** 所以到底什麼是tocken？我要怎麼得到它？我要花錢嗎？我剛買的tocken為何突然價值下跌了!?
3. **Complex:** 看了about page，我還是搞不清楚這個Dapp是做什麼的？好多專有名詞到底是什麼意思？
4. **Antisocial:** 介面顯示的並不是一個正常人類，而是一串hash code "0x1234..."，這到底是什麼？我根本不知道這address是不是我朋友
5. **Finality:** 有些使用者並沒有意識到在Dapp上的transaction往往是不可逆的，不能重來、沒有回到上一步，就算他們意識到了，也讓他們倍感焦慮
6. **Cost:** 使用這個Dapp居然還要付錢！？我根本還搞不清楚這Dapp在幹嘛，就要我花錢？
7. **Wait times:** 一個transaction的loading時間超長
8. **Fragmentation:** 我以為我已經建立了個人資料，為何還要我重建一次？那我之前建的跑去哪了？

<br/>
## Insights of building Web3 applications:
If you need users to do transaction, you shouldn't make them to pay. And they shouldn't have to worry about onboarding and buying tockens and acquiring Ether just to use your app. Users only need to know what this app is, what can they do with it, that’s all! They don’t have to know what’s working under the hood, do you think there are lots of people know the tech stack of facebook? NO! So you shouldn't expect users to know the existence of private keys. You can mask complex data with more user-friendly info.

<br/>
## How can we address some of these issues?
Michael Sena（3box Cofounder）建議應該從Dev tools中來建立Design Pattern，因為現在整個Web3還在非常早期發展階段，先將目標放在已具備些背景知識的開發人員，改善他們使用dev tools和protocal的user experience，從中發展出Userbility Approaches和Design Patterns，才能從根本解決問題，並且將經驗複製推移到一般使用者身上。Web3讓開發人員不必再擔心隱私或如何存儲用戶數據，因為使用者負責自己的數據，開發人員可以專注於提供更好的使用者體驗。不過同樣的，開發人員也有責任提供良好的使用者體驗，不能只一味求開發方便，就忽略使用者，開發人員有責任即使讓程式複雜，也要提供magical moments給使用者。

<br/>
## Rules for More Usable + Engaging Web3 Apps:
1. **Move off-chain whatever you can:** 除了比較重要的finacial transcation或必要的操作，其餘在Dapps上的操作能不跑Global state就不要跑(Minimal Viable Blockchain)，使用MetaTransactions, Sidechains or State channels to reduce runtime。
2. **Remove tokens whenever possible:** 盡量能不用代幣使用你的Dapp就不用，不要一開始就設門檻給使用者，讓使用者即使沒有tocken也能在他本來的Web2 browser load UI去使用你的Dapp，等到之後使用者連接其Etherium account，再unlock更多功能
3. **Use Web2 patterns when possible:** 整體來說，Web3還是令人感到陌生，能套用Web2的使用模式就盡量使用
4. **Think about your end users not robots. Create something people want or need.**
5. **Make things work together:** 隨時注意整個Web3生態系統中的應用和工具，讓你的Dapp能夠連結其他的工具

<br/>
## Tools for More Usable + Engaging Web3 Apps:
1. **Stable Tockens:** 使用低風險低成本的stable tockens，特別在onboarding new users時，讓他們能先用stable coins試用你Dapp的功能。ex:[Dai stablecoin](https://makerdao.com/en/dai/)
2. **Keyless Onboarding:** 在onboard new users時，讓他們使用暫時性的key(Ephemeral Keys)。ex:[Burner Wallets](https://github.com/austintgriffith/burner-wallet)
3. **Social Profiles + Data Storage:** 讓你的Dapp不要只是顯示Hash address，而是顯示個人profile。ex: [3box](https://3box.io/)
4. **Connecting Wallet and Dapps:** 輕鬆連結使用者的錢包和Dapp。ex: [WalletConnect](https://walletconnect.org/)

<br/>
## Further References:
[10 Usability Heuristics for UI Design in the Blockchain Era](https://mvpworkshop.co/10-usability-heuristics-for-ui-design-in-the-blockchain-era/)


