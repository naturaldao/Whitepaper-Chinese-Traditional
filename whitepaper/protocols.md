---
description: 各種治理協議的交聯是非常複雜的。
---

# PoV（價值證明）中的治理協議

如前所述，道易程PoV中有七大治理協議：

* 智能公器硬核协议（Smart Commons' Hardcore Protocol）
* 去中心化鑄造協議 Decentralized Minting Protocol
* 去中心化自治基金協議（Protocol of DAF，Protocol of Decentralized Autonomous Fund）
* 估值通證供應協議（Protocol of Valuation Token's Supply）
* 計量單位通證協議（Protocol of Unit Token）
* 去中心化交易協議（Protocol of Decentralized Exchange）
* 通用支付協議（Protocol of Universal Payment）

## 智能公器硬核协议（Smart Commons' Hardcore Protocol） <a href="#daohardcore" id="daohardcore"></a>

* 智能公器硬核協議涵括智能公器所需要的基礎資料如插槽ID、項目英文名稱、項目Logo（SVG格式，建議不超過6K，否則實在太貴）、項目描述（可以是宣傳口號Slogan）、創建時間（平台記錄）、創始成員（匿名，只是ETH地址），版本號，專屬估值通證的名稱、簡稱和符號等等。
* 在設置智能公器時，創建者可以手工添加一些地址到該智能公器作為其初始成員。
* 該協議還包含智能公器的升級規則：它的dApp必須是可靠的。這意味着它的dApp一旦部署就不能被任何人修改。

如果你知道使命是[智能合約的可組合性](https://ethereum.org/zh/developers/docs/smart-contracts/composability)，你就知道這條規則有多重要。從技術上講，代理模式（Proxy Pattern）對於幾乎所有智能公器來說都是一種自殺方式。如果您發現dApp中存在錯誤，請修復它並將其作為新的dApp部署到以太坊，然後返回道易程將其Mint為其智能公器的新版本。

因此，數據分離（Data Separation）可能是一些dApp開發的最佳策略，並且合約遷移（Contract Migration）也可能可行。

如果您需要一些幫助來了解dApp升級，[推薦閱讀本文](https://dev.to/joshuajee/smart-contract-upgrade-1ec2)。

## 去中心化鑄造協議 Decentralized Minting Protocol <a href="#deauthentication" id="deauthentication"></a>

鑄造（Minting）即是合約交互，它是智能合約間最基礎的行為。DAism摒棄了當前虛幻的DID概念，為smart common的創建採用了極簡且極為可靠的去中心化認證手段，即smart common的創建始於某個合約地址下的智能合約的Minting請求而與當前其它任何DID無關。Mint協議可以證明一個smart common源於哪個智能合約，而此智能合約即能讓所有人知道其功用或目的，機制非常簡單也絕對真實可靠。它是創建smart common的唯一方式，也可作為smart common的創世證據，解決智能體及其專屬的估值通證和dApp基於哪個核心智能合約的這一真實信息的關聯問題。

同時，該協議中還包含了一個智能公器子協議，其名稱為 SC0（意為Smart Commons 0）。即Minting操作，也就是宣布某個智能合約或某個dApp（某些智能合約的組合）自身成為以太坊的公共資源（Public Goods）——我們稱其為智能公器（Smart Common）。這也就是說，接受道易程治理的dApp，即為智能公器。

> **SC0 v0.1**
>
> 用一個dApp Mint一個Smart Common意味着它接受了本協議的排他治理。
>
> 我們都知曉dApp的所有者（或開發者或管理者）全部匿名這一事實。因為匿名，沒有誰可證明其為任何權利的享有者，也沒有誰可證明誰是任何責任的背負者。
>
> 1、接受道易程的治理。
>
> 2、無著作權\
> 匿名意味着其開發的dApp完全貢獻至公共領域，將其歸屬於智能公器（Smart Common），除能夠享受價值證明（Proof-of-Value）帶來的獎勵外，徹底放棄（割裂）所有其它權利，包括所有相關權利和鄰接權利。
>
> 3、無責任\
> 匿名意味着這個世界上，沒有（無法確定）誰對一個dApp及其專屬估值通證提供任何形式的擔保，沒有誰（無法確定）承擔任何連帶責任。
>
> 當使用或調用本dApp，或投資本智能公物專屬估值通證時，任何人不得暗示本智能公器或其關聯的任何人（所有者、開發者、管理者）為他或她的行為背書。

## **去中心化自治基金協議（Protocol of DAF，Protocol of Decentralized Autonomous Fund）** <a href="#daf" id="daf"></a>

道易程的價值證明給每個smart common都提供了可以永續的獎勵。每家smart common也都有一個極簡的去中心化自治基金（Decentralized Autonomous Fund），該 DAF 可以調整獎金的分配，包括分配給哪些賬戶、每個賬戶被分配的額度（百分數）。

## 估值通證供應協議（Protocol of Valuation Token's Supply） <a href="#tokensupply" id="tokensupply"></a>

任何一個智能公器都會發行其專屬的估值通證（中文也可以稱其為估值代幣）。估值通證的主要作用是讓投資者參與dApp的價值評估，並為道易程的共識價值證明提供獎金來源。

該協議主要定義估值通證的技術標準、名稱、縮略符、Logo及其發行量、發行價。

估值通證協議和IADD有非常密切的關係，可以說它也是構成 IADD 網絡的重要協議之一。

* 通證標準為EIP-3712。
* 估值通證全部發行到 IADD 網絡，項目方1個都沒有。它徹底革新了區塊鏈長期不合理的代幣市場供應機制，也是防範項目方和資本方聯合操控市場甚至空手套白狼忽悠市場的重要手段！
* 發行標準都一致：發行總量為1,000,000,000個，發行價為 0.000000000000000000 vita（類似天平的歸零。歸零前在算法里的價格是0.01 vita）。

## **計量單位通證協議（Protocol of Unit Token）** <a href="#utoken" id="utoken"></a>

此協議的目的是建立價格單位制！

計量單位通證是道易程的 IADD （去中心化交易和去中心化支付2合1網絡）中，通過恆定乘積算法（constant product formula），為一切估值通證定價的通證。

這是道易程的一個核心創新。該協議的核心是一種叫uToken（Unit Token的簡稱）的單位通證（價格原器）。

1. uToken 由 ETH 鍛造獲取，亦即定價通證有一個非常獨特的發行機制——你也可以理解為uToken是ETH的變體，其價值源於以太坊。uToken也是後面要介紹的 IADD 網絡核心要素。uToken也是IADD網絡的每一個交易對裡面的必需通證。
2. uToken 是一種非常獨特的通證。它是道易程定義的一種價格原器（單位通證），被定義為 1 uToken = 1 vita。和我們熟知的國際單位制的質量的基本單位類似，道易程有一套價格單位用於計算估值通證的價格。其中vita是通證價格的基本單位。
3. 道易程平台裡面的一切估值通證的即時價格，都以價格原器 uToken 為基準，以 vita為計價單位，通過恆定乘積算法（constant product formula）計算獲取。
4. vita是通證價格的基本單位。\
   計量通證 uToken 是道易程的去中心化交易和支付網絡（IADD網絡）中的價格原器（定價基準物），它的價格的基本單位為vita。那麼也就是說，凡涉及到通證交易或者支付時，一律以 vita為價格的基本單位來標價。就支付來說，通證經濟生態里的一切產品和服務的售價，也都以 vita為價格的基本單位來標價。如：\
   1 ISM = 0.01 vita\
   產品售價：0.5 vita/ kg\
   服務費：200 vita/ 小時

計量單位通證 uToken是道易程獨創的價格單位制里的幣價基準物。它會最大程度地降低代幣應用的覆雜度，也完全符合去中心化市場以及通用支付（結算）的需要。

### 為什麼我們需要ETH的變體？

* ETH 錯過了作為價格原型的機會，因為它的價值已經被美國的法定貨幣綁架了。 每當市場熊市的時候，一些礦工就因為ETH價格大幅下跌而不得不退出，充分說明了這一問題。
* ETH採用的發行策略不利於快速擴張的市場，因此它需要在短時間內大幅增加ETH的供應量。
* ETH是以太坊區塊鏈的原生加密貨幣，與智能合約發行的通證不同。 這意味着它不遵守 ERC-20 或任何其他通證標準，使得它通常必須在供 dApp 使用之前要先鑄造成 WETH（ERC-20 代幣）。為了解決這個問題，創建變體的最佳策略是通過鍛造。
* 在DAism的通證經濟學中，作為價格原型，uToken的價格是恆定的。 這使其成為投資結算或日常支付的理想代幣，類似於法定貨幣的日常使用。 與其他一些代幣不同，uToken 不能任意發行； 它需要有確定的價值來源。 此外，其發行必須遵循去中心化的方式以保持其信用。

### 計量單位通證協議簡介

該協議致力於價格單位制。這將是人類貨幣史上的一大創新！

在此協議中，基本價格單位為 vita，價格原器（定價基準物）為 uToken，也就是說一個 uToken的價格被定義為 1 vita。uToken的發行機制為ETH鍛造，其精度為18位。這也意味着價格的最小單位 attovita 是 vita 的 10^-18。

### 計量單位制：

**名稱：**計量單位通證（Unit Token）

**簡稱（**通證縮略符**）：**uToken

**標誌：**

<figure><img src="../.gitbook/assets/vita-s.svg" alt="" width="64"><figcaption></figcaption></figure>

**貨幣符號：**UTO

**基本單位：**vita

**輔幣進位制：**1vita=100cent（分)

**單位：**

|          |          |          |          |
| -------- | -------- | -------- | -------- |
| **表示因數** | **中文詞頭** | **英文前綴** | **詞頭符號** |
| 10^24    | 堯\[它]    | yotta    | Y        |
| 10^21    | 澤\[它]    | zetta    | Z        |
| 10^18    | 艾\[可薩]   | exa      | E        |
| 10^15    | 拍\[它]    | peta     | P        |
| 10^12    | 太\[拉]    | tera     | T        |
| 10^9     | 吉\[咖]    | giga     | G        |
| 10^6     | 兆        | mega     | M        |
| 10^3     | 千        | kilo     | k        |
| 10^2     | 百        | hecto    | h        |
| 10^1     | 十        | deca     | da       |
| 10^-1    | 分        | deci     | d        |
| 10^-2    | 厘        | centi    | c        |
| 10^-3    | 毫        | milli    | m        |
| 10^-6    | 微        | micro    | μ        |
| 10^-8    | 聰        | sat      | s        |
| 10^-9    | 納\[諾]    | nano     | n        |
| 10^-12   | 皮\[可]    | pico     | p        |
| 10^-15   | 飛\[母托]   | femto    | f        |
| 10^-18   | 阿\[托]    | atto     | a        |

### 計量單位通證協議的動機（Motivation）

要討論計量單位通證的意義，就離不開與它關系密不可分的 IADD 網絡。前面我們對 IADD Network的緣起已經解釋過。其中的重點為：

* 每個智能公器的估值通證都全部發行到 IADD 網絡。和現在普遍採用的代幣發售方式完全不同的是：項目方不負責估值通證發行、項目方也分配不到估值通證。杜絕項目方利用估值通證收割市場！
* 每個智能公器的估值通證都全部發行到了 IADD 網絡， IADD 里的估值通證的價格能夠反映市場的真實價值評判。

本協議的重點是價格單位制：

1. 國際單位制（法語：Système International d'Unités，簡稱SI）是世界上最普遍采用的標準度量系統。如1793年對重量（後改為質量）的定義為為冰點下體積為一立方分米的純水的重量。由此可見重量單位是通過一個參照物（標準物）定義出來的。而有了標準物及其基本單位，萬物的重量（質量）就都可以通過衡器中的算法算出來。計量單位通證是我們制定幣價單位制的價格原器（定價基準物）。
2. IADD 網絡採用了 Uniswap 的算法（恆定乘積方程式），但會以計量單位通證代替ETH來計算估值通證的價格。
3. ETH鍛造協議，通過鍛造ETH而發行出計量單位通證uToken，因此，uToken是ETH的變體——uToken不是憑空產生而是以ETH價值轉移而發行。這是一種去中心化鍛造模式，因為何時鍛造鍛造多少都是由用戶自己決定。
4. 道易程鍛造合約的啟動，將意味着以太坊的同質化通證第一次有了自己獨立自主的去中心化定價機制。也將意味着中心化世界的交易所對通證經濟生態的巧取豪奪的時代將要終結。
5. 計量單位通證的另一個重要的應用領域是去中心化結算。因其它一切代幣的價格都是波動的，無法被消費者持有而用於日常消費或者用於投資退出，只有uToken價格恆定（1 uToken ≡ 1 vita），因此它是道易程生態里合格的通用支付幣種（或稱結算幣種）。
6. 區塊鏈支付的需求是隨着區塊鏈行業的發展越來越大的，而我們今天又無法計算出未來某個年月它的需求的大小，因此我們需要一種發行量理論上無限的通用支付幣種。

這是一個志在徹底摧毀中心化交易所對去中心化市場的干擾和破壞的方案！也是一個區塊鏈結算的解決方案。

### 計量單位通證uToken的發行：ETH鍛造 <a href="#forge" id="forge"></a>

本節內容需要你預先了解Uniswap的恒定乘積算法。具體請參閱以下資料。

Hayden Adams. 2018：[https://hackmd.io/@477aQ9OrQTCbVR3fq1Qzxg/HJ9jLsfTz?type=view.](https://hackmd.io/@477aQ9OrQTCbVR3fq1Qzxg/HJ9jLsfTz?type=view.)

以及vitalik Buterin發起的討論：[Improving front running resistance of x\*y=k market makers](https://ethresear.ch/t/improving-front-running-resistance-of-x-y-k-market-makers/1281)

本項目將以**ETH鍛造**模式，以ETH的美元價格的历史最高值為參考發行計量單位通證uToken。精度18位，它的發行機制很獨特：

以CPMM改良算法（Imporved CPMM）為核心算法。

1. 鍛造初始化\
   協議啟動（即合約啟用）時，算法以每個計量單位通證所定義的價格即1 vita、ETH歷史最高價（當前為4870美元）為基礎進行初始化，即 1 ETH 可以鍛造出4870個uToken。
2.  改良的恆定乘積（Imporved CPMM）算法提供鍛造獎勵\
    核心算法還是Uniswap的恆定乘積方程式。\
    x: 鍛造池 ETH 數量\
    y: 鍛造池 uToken 數量\
    x \* y = k\
    第N位早鳥的獎勵R為：\
    $$R = Δy_{n} = y_{n-1} - y_{n}= (k \div x_{0}) - (k \div x_{1}) = k \times(1/x_{0}-1/x_{1})$$\
    其中\
    $$x_{n} = x_{n-1} + \Delta x_{n}$$

    $$\Delta x_{n}$$就是第n個人鍛造掉的ETH
3. 初始化K值\
   我們以至2022年11月30日 EIP-1559 已經burn掉的 ETH 為初始化的 ETH 總數。譬如我現在（20221130，00:00 香港時間）看到已經燒毀 2750240 個（[https://etherchain.org/burn](https://etherchain.org/burn)），其價值為：3320364758美元。這是全球用戶的損失，因此我們假設這些ETH都進入了鍛造池。\
   K = (2750240 \*3320364758)= 9,131,799,972,041,920 ≈ $9.1318e+15
4. 獎勵公式即為：\
   X \* Y = $9.1318e+15
5. 確定 ETH價格 再創新的最高價（假設為V2，之前的最高價假設為V1）的第二年，1個ETH 可鍛造的uToken數量即調整至該最高價的數值（即V2），所有歷史鍛造者均會獲得鍛造補償（即V2-V1）。\
   當鍛造的ETH達到其總量的60%，兌換基數不再增加。或者但ETH價格達到487000美元時，兌換基數（487000）不再增加。這是一個和外部市場的價格熔斷的機制。

## 去中心化交易協議（Protocol of Decentralized Exchange） <a href="#dex-pay" id="dex-pay"></a>

* 該協議治理的是估值通證的交易機制。
* 仍然採用Bancor創新的自動化做市商（Automated Market Maker, AMM）。價格發現機制與 Bancor Network 或 Uniswap 類似。即IADD網絡是道易程通用的去中心化交易和去中心化支付網絡。 道易程以定價通證uToken、智能公器專屬的估值通證、恆定乘積方程式、智能合約構成IADD網絡。
* 通過估值通證供應協議的協同，智能合約用算法獨立治理流動性池，無需人參與。
* 估值通證在 IADD 網絡有交易時，交易手續費（交易量的0.2%）作為獎金獎勵給其所屬智能公器的開發者。

## 通用支付協議（Protocol of Universal Payment）

與去中心化自治基金會協議、計量單位通證協議、去中心化交易協議密切配合。

一切產品與服務的價格均以 vita 為價格單位。

購買產品或服務時，通過 IADD Network 完成不同幣種的自動兌換。此時，uToken就是商家的結算通證。

## 其它與治理相關的技術探討

## **圖片存儲標準**

我們原創的圖片存儲標準意義重大：

* 首先應用於榮譽通證的鏈上存儲。我們成功制訂了[EIP-2569（Saving and Displaying Image Onchain for Universal Tokens）](https://eips.ethereum.org/EIPS/eip-2569)，即面向整個以太坊應用的技術標準。
* 擴大應用到一切圖片的存儲。譬如我們已經將它應用到了去中心化媒體。

### **榮譽通證（Token of Honor）** <a href="#honor" id="honor"></a>

榮譽的記錄和表彰，是智能公器發展的重要激勵手段。

榮譽通證的應用面是非常廣泛的，包含：

* 區塊鏈領域的榮譽勳章（Medal of Honor）、紀念幣（Commemorative Token）、紀念章、徽章、證書等等
* 具有收藏價值的遊戲道具等——也就是說我們的榮譽通證是百分之百保存在鏈上的（包括圖片）。

這是我們開發的簡單的榮譽通證交易所

[toh.best](https://toh.best)

或者測試網絡Ropsten里的DEMO：

[https://1155.goh.cool/](https://1155.goh.cool/)

[https://honor.goh.cool](https://honor.goh.cool/latest)

## **UI標準與協議 UI Standard & Protocol**

為便於第三方開發道易程應用層的模塊，我們未來還要提供UI標準。當然第三方貢獻也行。&#x20;

目前已確定使用的第三方協議有ActivityPub。
