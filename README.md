# 🐕 Dogecoin2 (DC2) - Official Repository & Node CLI Guide

Dogecoin2 is made in part for all the other crypto 2.0 projects emerging. This will be merged with LC2 just as the original doge is into Litecoin. Launched with the Doge 1.14.9 forked source using its own Genesis block.

---

## 🌐 Official Links & Ecosystem

Stay updated and engage with the official Dogecoin2 ecosystem through the following verified platforms:

* **Official Website:** [doge2.org](https://doge2.org/) | [dogecoin2.online](https://dogecoin2.online/)
* **Block Explorer:** [explorer.doge2.org](http://explorer.doge2.org/)
* **Live Exchange Trading:** [NestEx (DC2/USDT)](https://trade.nestex.one/spot/DC2)
* **Community Channels:** [Discord Invitation](https://discord.com/invite/5S3QQmD6A) | [Telegram Group](https://t.me/Dogecoin_II) | [X / Twitter @DogecoinII_DC2](https://x.com/DogecoinII_DC2)

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

