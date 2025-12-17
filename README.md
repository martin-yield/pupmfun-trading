# 🚀 **Copy trading Bot using Rust**

Welcome to the ** Copy trading Bot **! This bot watches for target wallet (whale) on the Solana blockchain in real-time, copy trading like target trading. 🌟



### 🎯 Example
- Source Transaction: https://solscan.io/tx/2nNc1DsGxGoYWdweZhKQqnngfEjJqDA4zxnHar2S9bsAYP2csbLRgMpUmy68xuG1RaUGV9xb9k7dGdXcjgcmtJUh
- Copied Transaction: https://solscan.io/tx/n2qrk4Xg3gfBBci6CXGKFqcTC8695sgNyzvacPHVaNkiwjWecwvY5WdNKgtgJhoLJfug6QkXQuaZeB5hVazW6ev
- Target Wallet: GXAtmWucJEQxuL8PtpP13atoFi78eM6c9Cuw9fK9W4na
- Copy Wallet: HqbQwVM2fhdYJXqFhBE68zX6mLqCWqEqdgrtf2ePmjRz
### 🎯 **Key Features**

- 🛰️ **Real-time WebSocket Streaming**:
  Connects to Solana's blockchain through Helius geyser RPC WebSocket and listens for new transactions, specifically Tx that target wallet is singer
- 🔍 **Filter Transactions**:
  Filters transactions as soon as possible and fast.
  maybe it takes about 0.3ms totally
- 📊 ** Make Copy transaction **:
  Using pumpfun program id and raydium module you can make copy trasaction.

---



1. **Install Dependencies**:

   Navigate to the project directory and run the following command:

   ```bash
   cd copy-trading-bot
   cargo build
   ```

2. **Configure ENV**:

   Replace the API token in the `ENDPOINT` variable:

   ```ts
   const ENDPOINT = "https://mainnet.helius-rpc.com";
   const WSS_ENDPOINT = "wss://atlas-mainnet.helius-rpc.com";
   const TARGET = "YOUR_API_TOKEN";
   ```

3. **Run the Bot**:

   Start the bot by running:

   ```bash
   cargo run
   ```

---
