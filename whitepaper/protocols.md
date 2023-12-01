---
description: ver 1.0 stable
---

# 道易程協議

如前所述，道易程PoV中有七大治理協議：

* DAO硬核協議（DAO Hardcore Protocol）
* 去中心化鑄造協議 Decentralized Minting Protocol
* 去中心化自治基金會協議（Protocol of DAF，Protocol of Decentralized Autonomous Fundation）
* 估值通證供應協議（Protocol of Valuation Token's Supply）
* 計量單位通證協議（Protocol of Unit Token）
* 去中心化交易協議（Protocol of Decentralized Exchange）
* 通用支付協議（Protocol of Universal Payment）

隨著道易程的發展，未來我們還可能會根據應用的需求而發展一些新的協議。

## **DAO硬核協議（去中心化自治智能體核心協議，DAO Hardcore Protocol）** <a href="#daohardcore" id="daohardcore"></a>

* DAO硬核協議涵括DAO所需要的基礎資料如智能體ID、項目英文名稱、項目Logo（SVG格式，建議不超過6K，否則實在太貴）、項目描述（可以是宣傳口號Slogan）、創建時間（平台記錄）、創始成員（匿名，只是ETH地址）、去中心化自治基金的合約地址，等等。
* 該協議可為該DAO的產品與服務提供去中心化認證。
* DAO硬核合約在應用層是可以拓展的。

DAO這種智能體有準入制度嗎？

我們相信DAO應該會采用完全開放的模式，即無需許可，大門敞開，界面和數據完全開放。它們基於開放透明的規則和智能算法來實現自我管理或被管理。

至於細則，我們認為需註意這些方面：

1. 如果沒有初始化核心共識，那麽一個DAO就沒法構造，因為這就意味著沒有人擁有任何權力。我們的策略是默認DAO的創建者為創始人或其授權人，創建者有權構造出一個DAO的輪廓（DApp列表及其設置、流通代幣的發行規劃等等）。請註意，創建時，我們會列出每個類別裏面的所有DApp，而不僅僅是核心DApp，供創建者自由組合。
2. 構建一家DAO的工作，包括項目的命名、ERC-20通證的發行、榮譽通證的去中心化認證、去中心化交易和支付網絡的自動部署等等。
3. 在設置DAO時，創建者可以手工添加一些地址到這家DAO作為這家的DAO的初始成員。所有這些地址都可供發行Cofounder榮譽頭銜勳章。地址暫定上限為100人。
4. 我們把去中心化共識決策的實現交給應用層的dApp去解決。
5. 默認情況下，該DAO的所有規則都是公開透明的。
6. 一個DAO創建成功，則自動獲得去中心化認證標識。
7. DAO 應該是公共的，它不歸任何人、任何註冊於鏈下的組織或企業所私有。

## 去中心化鑄造協議 Decentralized Minting Protocol <a href="#deauthentication" id="deauthentication"></a>

鑄造（Minting）即是合約交互，它是智能合約間最基礎的行為。DAism摒棄了虛幻的DID概念，為DAO的創建採用了極簡且極為可靠的去中心化認證手段，即DAO的創建始於某個合約地址下的智能合約的Minting請求而與其它任何DID無關。Mint協議可以證明一個DAO源於哪個智能合約，而此智能合約即能讓所有人知道其功用或目的，機制非常簡單也絕對真實可靠。它是創建DAO的唯一方式，也可作為DAO的創世證據，解決智能體及其發行的代幣和產品（如DApp）基於哪個核心智能合約的這一真實信息的關聯問題。

同時，該協議也是一個公共資源協議，即Minting操作，也就是宣布某個智能合約或某個dApp（某些智能合約的組合）自身成為以太坊的公共資源（Public Goods）————我們稱其為智能資產（Smart Property）。這也就是說，接受道易程治理的DAO/dApp，即為智能資產。

## **去中心化自治基金會協議（Protocol of DAF，Protocol of Decentralized Autonomous Fundation）** <a href="#daf" id="daf"></a>

每個DAO都需要一個可以永續的去中心化自治基金（Sustainable Decentralized Autonomous Fund, SDAF），道易程為這一目標提供了基礎：

* 道易程的智能合約為每家DAO提供其所需要的獨立的去中心化自治基金會，該基金會具有唯一的合約賬戶。
* 每家DAO的資金，都通過這個去中心化自治基金會來實現去中心化管理。譬如任何DAO的產品或服務賺的錢，都直接到 DAF 的賬戶上，而不會到任何個人賬上或其它合約賬上（因此對於一個良好的DAO，其DAF具有永續性）。
* DAF除了管理資金的核心外，還有與三大重要：投票權重數據庫、投票器、驗票器。項目方可通過自行開發也可以使用用第三方開發的模板和dApp拓展這三部分。
* 允許建立白名單和黑名單制度。用以保障基金的正常使用和安全。

## **流通通證供應暨代幣供應協議（Protocol of Token's Circulating Supply）** <a href="#tokensupply" id="tokensupply"></a>

任何一個DAO都可以發行其唯一的流通用通證即代幣（ERC20通證的簡稱，以下同）。流通用通證主要幫助構建其自治的經濟生態，為DAO的創建和運營打好經濟基礎。

該協議主要定義代幣的技術標準、名稱、縮略符、Logo以及代幣的發行量、發行價等發行機制。

流通用通證協議和IADD有非常密切的關系，可以說它也是構成 IADD 網絡的重要協議之一。

每家DAO的代幣分發與應用的治理規則如下：

* 通證標準為EIP-3712。
* 代幣全部發行到 IADD 網絡，項目方1個代幣都沒有。它徹底革新了區塊鏈不合理的代幣市場供應機制，也是防範項目方和資本方聯合操控市場甚至空手套白狼忽悠市場的重要手段！
* 發行標準都一致：發行總量為10,000,000,000個，發行價為 0.01 vita。
* 其代幣在 IADD 網絡有流動時，項目方以其代幣收取統一而合理的手續費（0.195%）。

## **計量單位通證協議（Protocol of Unit Token）** <a href="#utoken" id="utoken"></a>

本協議又叫維塔公約（Vitaic Convention）。

計量單位通證是道易程的 IADD （去中心化交易和去中心化支付2合1網絡）中，通過恒定乘積算法（constant product formula），為一切流通通證（ETH、20代幣等等）定價的通證。

這是道易程的一個核心創新。該協議的核心是一種叫uToken的單位通證。

1.  uToken 由 ETH 鍛造獲取，亦即定價通證有一個非常獨特的發行機制——你也可以理解為uToken是ETH的變體，其價值源於以太坊。uToken也是後面要介紹的 IADD 網絡核心要素。

    詳情請訪問“IADD網絡”部分的“[計量單位通證uToken的發行：ETH鍛造](https://dcn.naturaldao.io/whitepaper/iadd#forge)”
2. uToken 是一種非常獨特的代幣。它是道易程定義的一種價格基準物（單位通證），被定義為 1 uToken = 1 vita。和我們熟知的**國際單位制**的質量的基本單位類似，道易程有[一套價格單位](https://dcn.naturaldao.io/whitepaper/iadd#ji-liang-dan-wei-zhi)用於計算流通通證（代幣）的價格。其中vita是代幣**價格的基本單位**。
3. 道易程平台裏面的一切代幣（流通通證）的即時價格，都以計量通證 uToken 為基準物，以 vita為計價單位，通過恒定乘積算法（constant product formula）計算獲取。
4.  vita是價格的基本單位。\
    計量通證 uToken 是道易程的去中心化交易和支付網絡（IADD網絡）中的定價基準物，它的價格的基本單位為vita。那麽也就是說，凡涉及到代幣交易或者支付時，一律以 vita為價格的基本單位來標價。就支付來說，道易程生態裏的一切產品和服務的售價，也都以 vita為價格的基本單位來標價。如：\
    1 ISM = 0.01 vita\
    產品售價：0.5 vita/ kg\
    服務費：200 vita/ 小時

    更多細節請訪問“IADD網絡”的“[計量單位通證協議](iadd.md#utoken)”。

計量單位通證 uToken是道易程獨創的幣價基準物。它會最大程度地降低代幣應用的覆雜度，也完全符合去中心化市場的需要。

## 去中心化交易和支付協議（Protocol of Decentralized Exchange and Decentralized Payment） <a href="#dex-pay" id="dex-pay"></a>

* 該協議治理的是代幣的交易和支付規則。
* IADD網絡是道易程通用的去中心化交易和去中心化支付網絡。 道易程以定價通證uToken、DAO專屬的代幣、恒定乘積方程式、智能合約構成IADD網絡。
* DAO專屬的代幣遵循流通通證供應暨代幣供應協議，發行時全部直接供應到IADD網絡。
* 代幣在 IADD 網絡有流動時，其所屬DAO收取0.195%作為流動手續費。道易程同時再收取0.005%。
* 如果該DAO沒有發行代幣，則它收費時直接收取 uToken。

## **榮譽通證協議（Token of Honor Protocol）** <a href="#honor" id="honor"></a>

榮譽的記錄和表彰，是DAO發展的重要激勵手段。它不是道易程的核心協議，而是道易程dApp市場裏的一個dApp所采用的協議。

榮譽通證的應用面是非常廣泛的，包含：

* 區塊鏈領域的榮譽勳章（Medal of Honor）、紀念幣（Commemorative Token）、紀念章、徽章、證書等等
* 大多具有收藏價值——也就是說我們的榮譽通證是百分之百保存在鏈上的（包括圖片）。

目標：

* 該協議定義榮譽通證的基礎發行標準
* 該協議定義榮譽通證的交易接口

這是我們開發的簡單的榮譽通證交易所的DEMO：

[https://1155.goh.cool/](https://1155.goh.cool/)

[https://honor.goh.cool](https://honor.goh.cool/latest)\*\*\*\*

## **圖片存儲標準**

我們原創的圖片存儲標準意義重大：

* 首先應用於榮譽通證的鏈上存儲。我們成功制訂了EIP-2569（Saving and Displaying Image Onchain for Universal Tokens），以太坊已經收錄（查詢：[https://eips.ethereum.org/all](https://eips.ethereum.org/all)）。這意味著我們創立了面向整個以太坊應用的技術標準。
* 擴大應用到一切圖片的存儲。譬如我們已經將它應用到了去中心化媒體。

## **DApp接口標準與協議 Standards and Protocols for DApp Interfaces**

DAO的應用層就是各種擴展應用（也就是DAO功能的封裝和擴展，我們稱之為“DApp”），以及可能的獨立Dapp。

包含：

* 第三方DApp的拓展接口。
* 第三方DApp的協議（DDIP，DAism dAPP Improvement Protocol）

## **UI標準與協議 UI Standard & Protocol**

為便於第三方開發道易程應用層的模塊，我們未來還要提供UI標準。當然第三方貢獻也行。

目前已確定的有 Monkey King Protocol。
