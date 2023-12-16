---
description: 各種治理協議的交聯是非常複雜的。
---

# PoV（價值證明）中的治理協議

如前所述，道易程PoV中有七大治理協議：

* DAO硬核協議（DAO Hardcore Protocol）
* 去中心化鑄造協議 Decentralized Minting Protocol
* 去中心化自治基金會協議（Protocol of DAF，Protocol of Decentralized Autonomous Fundation）
* 估值通證供應協議（Protocol of Valuation Token's Supply）
* 計量單位通證協議（Protocol of Unit Token）
* 去中心化交易協議（Protocol of Decentralized Exchange）
* 通用支付協議（Protocol of Universal Payment）

隨著道易程的發展，未來我們還可能會根據應用的需求而發展一些新的協議。

## **DAO硬核協議（DAO Hardcore Protocol）** <a href="#daohardcore" id="daohardcore"></a>

* DAO硬核協議涵括DAO所需要的基礎資料如插槽ID、項目英文名稱、項目Logo（SVG格式，建議不超過6K，否則實在太貴）、項目描述（可以是宣傳口號Slogan）、創建時間（平台記錄）、創始成員（匿名，只是ETH地址），專屬估值通證的名稱、簡稱和符號等等。
* 在設置DAO時，創建者可以手工添加一些地址到這家DAO作為這家的DAO的初始成員。地址上限為64人。
* 該協議還包含DAO的升級規則。

## 去中心化鑄造協議 Decentralized Minting Protocol <a href="#deauthentication" id="deauthentication"></a>

鑄造（Minting）即是合約交互，它是智能合約間最基礎的行為。DAism摒棄了當前虛幻的DID概念，為DAO的創建採用了極簡且極為可靠的去中心化認證手段，即DAO的創建始於某個合約地址下的智能合約的Minting請求而與當前其它任何DID無關。Mint協議可以證明一個DAO源於哪個智能合約，而此智能合約即能讓所有人知道其功用或目的，機制非常簡單也絕對真實可靠。它是創建DAO的唯一方式，也可作為DAO的創世證據，解決智能體及其專屬的估值通證和產品（如DApp）基於哪個核心智能合約的這一真實信息的關聯問題。

同時，該協議中還包含了一個智能資產子協議，其名稱為 SC0（意為Smart Commons 0）。即Minting操作，也就是宣布某個智能合約或某個dApp（某些智能合約的組合）自身成為以太坊的公共資源（Public Goods）——我們稱其為智能公物（Smart Commons）。這也就是說，接受道易程治理的dApp，即為智能公物。

> **SC0 v0.1**
>
> 用一個dApp Mint一個 DAO 意味着該dApp接受本協議成為其唯一協議，也接受其所有者和管理者（我們稱之為DAO的成員）全部匿名這一事實。
>
> 因為匿名，無人可證明某人是任何權利的享有者，也無人可證明某人是任何責任的背負者。
>
> 1、無著作權\
> 匿名意味着其開發的dApp完全貢獻至公共領域，將其歸屬於智能公物（Smart Commons），除能夠享受價值證明（Proof-of-Work）帶來的獎勵外，徹底放棄所有其它權利，包括所有相關權利和鄰接權利。
>
> 2、無責任\
> 匿名意味着這個世界上，沒有誰對一個dApp及其專屬估值通證提供任何形式的擔保，沒有誰承擔任何連帶責任。
>
> 當使用或調用本dApp，或投資本DAO專屬估值通證時，任何人不得暗示本DAO或其任何聲明者為他或她的行為背書。

## **去中心化自治基金會協議（Protocol of DAF，Protocol of Decentralized Autonomous Fundation）** <a href="#daf" id="daf"></a>

道易程的價值證明給每個DAO都提供了可以永續的獎勵。每家DAO也都有一個極簡的去中心化自治基金會（Decentralized Autonomous Fundation），該 DAF 可以調整獎金的分配，包括分配給哪些賬戶、每個賬戶被分配的額度（百分數）。

## 估值通證供應協議（Protocol of Valuation Token's Supply） <a href="#tokensupply" id="tokensupply"></a>

估值通證供應也叫哈耶克公約一（Hayek Convention No.1）。

任何一個DAO都會發行其專屬的估值用通證（中文也可以稱其為估值用代幣）。估值通證的主要作用是讓投資者參與dApp的價值評估，並為道易程的共識價值證明提供獎金。

該協議主要定義估值通證的技術標準、名稱、縮略符、Logo及其發行量、發行價。

估值通證協議和IADD有非常密切的關係，可以說它也是構成 IADD 網絡的重要協議之一。

* 通證標準為EIP-3712。
* 估值通證全部發行到 IADD 網絡，項目方1個都沒有。它徹底革新了區塊鏈長期不合理的代幣市場供應機制，也是防範項目方和資本方聯合操控市場甚至空手套白狼忽悠市場的重要手段！
* 發行標準都一致：發行總量為10,000,000,000個，發行價為 0.000000000000000000 vita。

## **計量單位通證協議（Protocol of Unit Token）** <a href="#utoken" id="utoken"></a>

本協議也叫哈耶克公約二（Hayek Convention No.2）。

計量單位通證是道易程的 IADD （去中心化交易和去中心化支付2合1網絡）中，通過恆定乘積算法（constant product formula），為一切估值通證定價的通證。

這是道易程的一個核心創新。該協議的核心是一種叫uToken（Unit Token的簡稱）的單位通證（價格原器，價格基準物）。

1.  uToken 由 ETH 鍛造獲取，亦即定價通證有一個非常獨特的發行機制——你也可以理解為uToken是ETH的變體，其價值源於以太坊。uToken也是後面要介紹的 IADD 網絡核心要素。

    詳情請訪問“IADD網絡”部分的“[計量單位通證uToken的發行：ETH鍛造](https://dcn.naturaldao.io/whitepaper/iadd#forge)”
2. uToken 是一種非常獨特的代幣。它是道易程定義的一種單位通證（價格原器，價格基準物），被定義為 1 uToken = 1 vita。和我們熟知的**國際單位制**的質量的基本單位類似，道易程有[一套價格單位](https://dcn.naturaldao.io/whitepaper/iadd#ji-liang-dan-wei-zhi)用於計算估值通證（代幣）的價格。其中vita是代幣**價格的基本單位**。
3. 道易程平台裡面的一切估值通證的即時價格，都以計量通證 uToken 為單位通證（價格原器，價格基準物），以 vita為計價單位，通過恆定乘積算法（constant product formula）計算獲取。
4.  vita是通證價格的基本單位。\
    計量通證 uToken 是道易程的去中心化交易和支付網絡（IADD網絡）中的定價基準物，它的價格的基本單位為vita。那麽也就是說，凡涉及到通證交易或者支付時，一律以 vita為價格的基本單位來標價。就支付來說，道易程生態裏的一切產品和服務的售價，也都以 vita為價格的基本單位來標價。如：\
    1 ISM = 0.01 vita\
    產品售價：0.5 vita/ kg\
    服務費：200 vita/ 小時

    更多細節請訪問“IADD網絡”的“[計量單位通證協議](iadd.md#utoken)”。

計量單位通證 uToken是道易程獨創的價格單位制里的幣價基準物。它會最大程度地降低代幣應用的覆雜度，也完全符合去中心化市場以及通用支付（結算）的需要。

## 去中心化交易協議（Protocol of Decentralized Exchange） <a href="#dex-pay" id="dex-pay"></a>

* 該協議治理的是估值通證的交易機制。
* 仍然採用Bancor創新的自動化做市商（Automated Market Maker, AMM）。價格發現機制與 Bancor Network 或 Uniswap 類似。即IADD網絡是道易程通用的去中心化交易和去中心化支付網絡。 道易程以定價通證uToken、DAO專屬的估值通證、恆定乘積方程式、智能合約構成IADD網絡。
* 通過估值通證供應協議的協同，智能合約用算法獨立治理流動性池，無需人參與。
* 估值通證在 IADD 網絡有交易時，交易手續費（0.2%）作為獎金獎勵給其所屬DAO。

## 通用支付協議（Protocol of Universal Payment）

與去中心化自治基金會協議、計量單位通證協議、去中心化交易協議密切配合。

一切產品與服務的價格均以 vita 為價格單位。

購買產品或服務時，通過 IADD Network 完成不同幣種的自動兌換。此時，uToken就是商家的結算通證。

## 其它與治理相關的技術探討

## **圖片存儲標準**

我們原創的圖片存儲標準意義重大：

* 首先應用於榮譽通證的鏈上存儲。我們成功制訂了EIP-2569（Saving and Displaying Image Onchain for Universal Tokens），以太坊已經收錄（查詢：[https://eips.ethereum.org/all](https://eips.ethereum.org/all)）。這意味著我們創立了面向整個以太坊應用的技術標準。
* 擴大應用到一切圖片的存儲。譬如我們已經將它應用到了去中心化媒體。

### **榮譽通證（Token of Honor）** <a href="#honor" id="honor"></a>

榮譽的記錄和表彰，是DAO發展的重要激勵手段。

榮譽通證的應用面是非常廣泛的，包含：

* 區塊鏈領域的榮譽勳章（Medal of Honor）、紀念幣（Commemorative Token）、紀念章、徽章、證書等等
* 具有收藏價值的遊戲道具等——也就是說我們的榮譽通證是百分之百保存在鏈上的（包括圖片）。

這是我們開發的簡單的榮譽通證交易所的DEMO：

[https://1155.goh.cool/](https://1155.goh.cool/)

[https://honor.goh.cool](https://honor.goh.cool/latest)

## **UI標準與協議 UI Standard & Protocol**

為便於第三方開發道易程應用層的模塊，我們未來還要提供UI標準。當然第三方貢獻也行。&#x20;

目前已確定使用的第三方協議有 Monkey King Protocol、ActivityPub。
