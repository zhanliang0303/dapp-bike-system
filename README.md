# 🚲 Blockchain Bike Rental System (區塊鏈單車租賃系統)

這是一個基於 **Sepolia 測試鏈** 的去中心化應用程式 (DApp)。使用者可以透過 MetaMask 錢包支付 ETH 租借單車，並在還車時透過智能合約自動取回押金。

## 🌟 專案特色 (Features)
* **錢包串接**：支援 MetaMask 登入與交易簽署。
* **透明租賃**：租金與押金機制寫在智能合約中，公開透明。
* **自動退款**：還車時，系統自動將 `0.005 ETH` 押金退回用戶錢包。
* **即時狀態**：前端介面即時同步區塊鏈上的交易狀態 (Loading/Success)。

## 🛠️ 技術使用 (Tech Stack)
* **Blockchain**: Ethereum (Sepolia Testnet)
* **Smart Contract**: Solidity
* **Frontend**: HTML, CSS, JavaScript (Web3.js)
* **Tools**: Remix IDE, MetaMask

---

## 📖 使用教學 (User Guide)

### 1. 連接錢包 (Connect Wallet)
進入網頁後，系統會自動偵測並請求連接 MetaMask 錢包。請確認您的網路已切換至 **Sepolia Testnet**。

### 2. 租借單車 (Rent a Bike)
點擊介面上的 **「租借單車」** 按鈕。
* **總費用**：`0.006 ETH` (包含 `0.001` 租金 + `0.005` 押金)
* MetaMask 會跳出交易確認視窗，請點擊 **「確認」**。

*(這裡可以拖拉進去你的截圖 1: 租借畫面)*

### 3. 等待上鏈 (Transaction Processing)
交易送出後，介面會顯示 **「租借中...」** 的動畫。此時正在等待區塊鏈確認交易。

### 4. 騎乘與還車 (Ride & Return)
交易成功後，狀態會更新為 **「已租借會員」**。
當您使用完畢，點擊 **「還車並取回押金」**。

### 5. 成功退款 (Refund Success)
確認還車交易後，系統會跳出通知，並將 **`0.005 ETH`** 押金自動退回您的錢包！🎉


---

## 📝 License
MIT License
