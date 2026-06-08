# 🐕 Dogecoin2 (DC2) - Official Repository & Node CLI Guide

Dogecoin2 is made in part for all the other crypto 2.0 projects emerging. This will be merged with LC2 just as the original doge is into Litecoin. Launched with the Doge 1.14.9 forked source using its own Genesis block.

---

## 🌐 Official Links & Ecosystem

Stay updated and engage with the official Dogecoin2 ecosystem through the following verified platforms:

| Category | Links |
|----------|-------|
| **Official Website** | [doge2.org](https://doge2.org/) \| [dogecoin2.online](https://dogecoin2.online/) |
| **Block Explorer** | [explorer.doge2.org](http://explorer.doge2.org/) |
| **Live Exchange** | [NestEx (DC2/USDT)](https://trade.nestex.one/spot/DC2) |
| **Community** | [Discord](https://discord.com/invite/5S3QQmD6A) \| [Telegram](https://t.me/Dogecoin_II) \| [X / Twitter](https://x.com/DogecoinII_DC2) |

---

## 📊 Technical Specifications (Node Core Engine)

Based on runtime diagnostic queries from the node daemon binary `v0.0.7`, the Dogecoin2 network structural properties are defined as follows:

| Network Parameter | Configured Value | Functional Impact & Description |
| :--- | :--- | :--- |
| **Wallet Architecture** | HD Wallet (`hdmasterkeyid`) | Hierarchical Deterministic engine. All addresses and change keys derive from a singular master seed ID. |
| **Minimum Relay Fee** | `0.00100000` DC2 | Ultra-low fee parameters for transaction broadcasting, optimized for micro-transactions. |
| **Hard Dust Limit** | `0.00100000` DC2 | The absolute minimal threshold allowed per output before transaction is labeled as spam/dust. |
| **Blockchain Size** | ~46 Megabytes (MB) | Freshly spun blockchain, enabling near-instant validation and rapid sync environments on cloud platforms. |

---

## ⛏️ Mining Mechanism & Block Reward

Dogecoin2 uses **Scrypt** as its Proof-of-Work algorithm with **Auxiliary Proof-of-Work (AuxPoW)** support, enabling **merge mining** with other Scrypt-based blockchains (like Litecoin).

### 🔐 Algorithm & Consensus

| Aspect | Detail |
| :--- | :--- |
| **Hash Algorithm** | Scrypt |
| **Consensus Mechanism** | AuxPoW (Merge Mining) |
| **Chain ID** | `0x1d37` |
| **Target Block Time** | 60 seconds (1 minute) |
| **Difficulty Algorithm** | Digishield (adjusts every block, activated at block 300) |
| **Halving Interval** | Every 100,000 blocks |

### 🪙 Block Reward Structure

The block reward follows a 3-era system based on block height:

| Period | Block Height | Halvings | Reward per Block |
| :--- | :--- | :--- | :--- |
| **1** | 0 - 100,000 | 0 | **500,000 DC2** |
| **2** | 100,001 - 200,000 | 1 | 250,000 DC2 |
| **3** | 200,001 - 300,000 | 2 | 125,000 DC2 |
| **4** | 300,001 - 400,000 | 3 | 62,500 DC2 |
| **5** | 400,001 - 500,000 | 4 | 31,250 DC2 |
| **6** | 500,001 - 600,000 | 5 | 15,625 DC2 |
| **7+** | ≥ 600,000 | - | 10,000 DC2 (constant inflation) |

> **Note:** The genesis block reward is also **500,000 DC2** (Period 1).

### ⚙️ How to Mine Dogecoin2

Since Dogecoin2 supports **AuxPoW (Merge Mining)** , you can mine DC2 **without additional hashing power** while mining other Scrypt coins like Litecoin.

#### Requirements:
- **Hardware:** Scrypt ASIC miner (e.g., Antminer L7, Elphapex DG1+, DG2)
- **Mining Pool:** Any pool that supports merge mining with chain ID `0x1d37`
- **Wallet:** A Dogecoin2 wallet address


## 🛠️ Network Connectivity & Static Nodes (Addnode)

If your node client encounters sync bottlenecks or displays `0 active connections`, apply these official seed nodes and global peer IP points directly inside your `dogecoin2.conf` profile or issue them through the CLI utility:

### Official DNS & Core Seed Nodes:
* `doge1.doge2.org` (Europe Node)
* `doge2.doge2.org` (Europe Node)
* `doge3.doge2.org` (DNS Crawler)

### Global Reliable IP Entry Nodes:
```ini
addnode=31.220.96.220:22023  # America
addnode=82.197.67.235:22023  # America
addnode=45.76.148.54:22023   # Asia

