# Solana Multi Dex Volume Booster

This is designed to increase the trading volume of any Solana token that has liquidity pools on Solana, across any DEX. It utilizes the **Jupiter** service to execute token swaps, and the **Jito** service for efficient transaction bundling. The bot supports highly customizable transaction parameters and multi-wallet configurations for maximum flexibility and control.

## ✨ Features

### - **Speed of Transaction (Per Minute)**: Set the transaction speed to execute a specific number of transactions per minute.
### - **Buy to Sell Ratio**: Define a ratio of buy to sell orders. The number of buy orders per transaction is determined by the ratio, with a random number of buy orders between 1 and the ratio value.
### - **Swap Amount Range**: Configure the minimum and maximum swap amounts for the buy orders in SOL, ensuring flexible trade sizes.
### - **Total Amount Distribution**: The total amount to be traded is distributed across 4 sub-wallets, each participating in the trading process.
### - **Jito Service Integration**: Executes all buy and sell transactions in a single block for efficiency and minimal gas consumption.
### - **Multi-Wallet Support**: The total trade amount is split between 4 sub-wallets, each performing the buy/sell process independently.
### - **Per-Wallet Control**: Trading can be turned on/off for each wallet individually.

## 🏗️ How it Works

1. **Set Transaction Parameters**:
   - Define transaction speed (transactions per minute).
   - Set the buy-to-sell ratio.
   - Configure the swap amount range (min, max) for each buy transaction.
   - Distribute the total trade amount across 4 wallets.

2. **Transaction Process**:
   - Each transaction contains multiple buy orders and a single sell order.
   - The number of buy orders is determined randomly based on the ratio.
   - Each buy amount is randomly selected within the predefined swap range.
   - Once all the buy orders are complete, a sell order is executed.
   - All transactions are bundled into a single block using **Jito** for maximum efficiency.

3. **Multi-Wallet Trading**:
   - The total trading amount is split between 4 sub-wallets.
   - Each sub-wallet executes its own buy/sell transactions following the same parameters.
   - The trading process for each wallet can be controlled independently (on/off).

## ⚙️ Customize

### - **Wallet Counts**: User can set wallet counts as you want
### - **Select Specific Dex**: User can select specific dex where as you want boost


## 📞 Contact Info

### Telegram: [enlomy](https://t.me/enlomy)

## 🍵 Tip

### If you are intereseted in my projects, please 🔗fork or give me ⭐star
