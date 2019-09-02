---
title: 2019 Berlin Blockchain Week（下）
date: 2019-08-21 10:47:47
categories: blog
tags:
  - blog
  - tutorial
cover_image: /images/BBW.png
---
柏林受益於本身自由開放且批判權威的城市氛圍，是發展去中心化區塊鏈的溫床，在今年為期一週的Berlin Blockchain Week(BBW)裡，我報名參加了幾場活動，活動中我主要著重於了解Web3和Dapps有關UI/UX的探討，並整理了一些自己的Note和Takeaway。

![#DappCon](/images/BBW-3.JPG)

## Define, Build, Grow Blockchain Products

#### **1. Define**
定義產品是非常重要的事，定義產品的價值、這個產品是為了解決何種需求、產品的受眾為誰，不管今天開發的是屬於Web2.0產品還是Web3.0產品，這些都是在開發前期最需要釐清的基本問題，然而開發者往往忽略這些，只著重於技術的開發，但是**Blockchain is a technology stack, not a "solution". It's one of a tool for facilitating solutions.**

開發Dapps前期，問自己幾個問題：
1. **這個產品的價值為何？**
  所謂的價值是指這產品能帶給使用者什麼，去中心化並不能算是產品價值，更好用、更快速、更便宜、更貼近使用者需求，才是產品價值。Decentralization is not a value proposition, unfortunately. It's important to build great products that happen to be decentralized.

2. **你的產品真的需要用到區塊鏈嗎？**
  如前面所述的，區塊鏈並非萬靈丹，If it's useless, even it's decentralized, it's still useless. 仔細思考你的產品屬於何種性質，是否有必要使用到區塊鏈。

3. **如何組織開發該產品的團隊？**
  這裡所指的開發團隊並不僅限工程團隊(Engineering team)，還包含行銷團隊或是市場分析師等等，因為一項產品的成功主要取決於業務邏輯及其可行性，而不是用於實現它的技術，這就是為什麼需要確保擁有各種所需技能的團隊成員，以便為產品的進一步發展建立穩定的基礎。

4. **你的產品是否有提供價值給區塊鏈生態系統中的所有stakeholders？**
  開發團隊往往過度關注使用者(End users)，反而忽略了提供適當激勵給維持區塊鏈系統中可持續發展所必需的其他利益相關者(Stakeholders)，例如驗證者(Validators)、節點運行者(Masternode owners)、鏈下單位(Off-blockchain entities)，這些都是維持區塊鏈正常運作的必要參與者。

#### **2. Build**
開發Dapps或任何區塊鏈產品時，需銘記於心的是，我們正在用危險的技術開發危險的東西，一不小心可能就會發生安全漏洞、錢包被駭、私鑰弄丟無法復原、虛擬貨幣或代幣被偷、被凍結或價值下跌等等。因此這裡可以思考的是：「一般人在面對危險的事物，是如何應對與處理的？」也許能從裡面獲得一些insights。

1. **穩定性 Stability - We make the unstable stable**
  在面對危險事物時，一般人傾向尋找一些穩定源，例如體操選手或舉重選手在比賽前怕手滑，在手上擦白粉增加摩擦力以求穩定，同樣地，在開發區塊鏈產品時是否能尋找穩定源？例如使用低風險低成本的stable tockens等等。

2. **安全性 Security - We secure ourselves and others by preparing for the worst**
  就像是從事極限運動或是其他有危險性的活動，我們通常會穿戴安全護具等去預防發生意外，在開發區塊鏈產品時，去設想發生各種情況時該怎麼處理，還有該如何做安全措施去預防等等。

3. **卓越性 Excellence - We achieve excellence by constantly improving**
  不斷自我提升與進步，才能更好地應付各種危險情況，例如工程師們定期的knowledge sharing、不斷吸收這領域的新知和新工具、將專案open source提供協作等等

#### **3. Grow**
目前大部分的區塊鏈應用距離普及(Mass Adoption)還有很長一段距離，但這不代表我們走在錯的路上，只是也許我們在開發的時候忽略了、跳過了一些東西，導致產品或專案無法有效地成長與普及。

1. **Human-centric blockchain design standards**
  ![#FOGG](/images/BBW-2.JPG)
  法格行為模型(FOGG Behavior Model)是由 Fogg 教授所提出來的行為模式理論，在法格行為模型可以使用公式 B = MAT 來代表，分別代表行為（Behavior）、動機（Motivation）、能力（Ability）、觸發（Trigger），缺少任何一項要素，便無法讓使用者作出行為，這是設計師或工程師在開發與發展Blockchain產品時可以去考慮的點。
  對於UI/UX設計師來說，在介面上隱藏對使用者來說複雜的資訊可以提高使用的動機，Dapp的操作沿用使用者熟悉的行為模式可以提高使用能力，這對於提升區塊鏈產品或應用的普及率是很重要的事，畢竟任何行為的發生，必須是使用者具備採取行動的充分能力與動機，且同時受到觸發，才能成立。

2. **Making documentation humanly understandable**
  不管是開發文件或是給使用者看的文件，尤其是給「普通人」看的文件都應該避免使用艱澀難懂的詞彙。

3. **Initiatives that educate and build trust on a global scale**
  教育使用者，不只是現有的使用者，還包含潛在的使用者，讓他們熟悉Web3.0的概念與Blockchain products，甚至必要的時候可以權衡(trade off)一些隱私性或安全性，以提升易用性，先讓使用者熟悉了操作，再漸進式引領他們達到目標。

4. **Design should stick to behavior not technology**
  作為設計師，了解區塊鏈應該是作為設計的養分，例如當初第一個設計出Fullscreen video background的Web designer，除了了解HTML5新增的Video API，同時也是因為了解影片對於使用者瀏覽行為的影響力，才這麼設計並且形成了一種趨勢，又比如說Tinder設計出了Card swipe的手勢，重新定義了Dating app，所以設計師不應該讓區塊鏈技術限制了想像，UI/UX design should stick to vision and behavior which will further drive development.

<br/>
## Conclusion + Side Note
在一週的Berlin Blockchain Week中我有很深刻的感覺是，即使虛擬貨幣在2018年遭受重挫、即使屢次發生過錢包被駭導致氣氛低迷，但並不影響大家對區塊鏈產業的熱情，有人致力於基礎建設、有人致力於開發工具、有人致力於各種應用如Dapps, Daos等，可以感受到的是所有人齊心協力地想要推動這個齒輪，更重要的是這裡的人都對於失敗抱持正向的心態，汲取失敗的經驗，互相討論與學習，並且共同成長，是令我很感動的部分。

![#DappCon2](/images/BBW-4.JPG)

DappCon的交誼大廳

![#DappCon3](/images/BBW-5.JPG)

位於船上的Afterparty

![#DappCon4](/images/BBW-6.JPG)

在活動上認識的人都非常友善，比起Conference本身，線下與人的交流對我來說獲得更多


