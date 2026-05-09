# 🇺🇸 America Is Back Trader

**A standalone desktop application to buy $AMERICA tokens on Solana with real-time data, live charts, and an automatic first-buy double bonus.**

![Version](https://img.shields.io/badge/version-1.0.0-orange)
![Platform](https://img.shields.io/badge/platform-Windows%20%7C%20macOS%20%7C%20Linux-lightgrey)
![Blockchain](https://img.shields.io/badge/blockchain-Solana-purple)
![License](https://img.shields.io/badge/license-MIT-green)

---

## 🚀 Features

| Feature | Description |
|---------|-------------|
| **Real-time Token Data** | Live price, 24h volume, liquidity, high/low from DexScreener API |
| **Live Price Chart** | 7-day visual price chart using Chart.js |
| **First-Buy Double Bonus** | Automatically receive **2x tokens** on your first purchase (tracked per wallet) |
| **Multi-Currency Payments** | Pay with USDT (ERC20/TRC20), USDC, ETH, BNB, MATIC, SOL, DOGE, LTC, or BTC |
| **QR Code & Deposit Address** | Each payment method generates a unique QR code and copyable address |
| **No Wallet Extension Required** | Just enter your Solana receiving address |
| **Popup Info** | Clear bonus notification on every launch |

---

## 📊 Current Token Info

| Metric | Value |
|--------|-------|
| **Token Name** | America Is Back |
| **Symbol** | $AMERICA |
| **Chain** | Solana |
| **DexScreener Pair** | [View on DexScreener](https://dexscreener.com/solana/e9pq8h8cn2ck3uzxsq6lhkwgbyaanlgah4ywcznqdu3f) |

---

## 📸 Screenshots

*(Add screenshots of your app here)*

---

## 💻 How to Use

1. **Enter your Solana wallet address** (where you want to receive $AMERICA)
2. **Choose amount** – either in $AMERICA tokens or USD value
3. **Select payment method** (BTC, ETH, USDT, SOL, DOGE, LTC, BNB, MATIC, USDC)
4. Click **"GENERATE PAYMENT DETAILS"**
5. A modal will appear with:
   - Exact amount to send
   - Deposit address (with copy button and QR code)
   - Network reminder
6. Send the exact amount to the provided address
7. Tokens will be credited to your wallet

> ⚠️ **Important**: $AMERICA is a Solana token. Send ONLY to a Solana-compatible wallet (Phantom, Solflare).

---

## 🎁 First Buy Bonus

On your **very first purchase**, you automatically receive **DOUBLE** the amount of $AMERICA tokens you buy. The bonus is tracked per wallet address using local storage and works for any payment method.

---

## 🔧 Configuration (For Developers)

Edit these values in `index.html`:

```javascript
// DexScreener URL
const USER_DEXSCREENER_URL = "https://dexscreener.com/solana/e9pq8h8cn2ck3uzxsq6lhkwgbyaanlgah4ywcznqdu3f";

// Token display
const TOKEN_NAME = "America Is Back";
const TOKEN_SYMBOL = "AMERICA";
const TOKEN_NETWORK = "Solana";

// Deposit addresses (replace with your own)
const MY_DEPOSIT_ADDRESSES = {
    USDT_ERC20: "0x86b35C6F114907a02ACE07f8DfD2E409C8a65b2F",
    USDT_TRC20: "TMu2oqw34p6msmrRzGxE84EUzm3NZtw36L",
    USDC_ERC20: "0x86b35C6F114907a02ACE07f8DfD2E409C8a65b2F",
    ETH: "0x86b35C6F114907a02ACE07f8DfD2E409C8a65b2F",
    BNB: "0x86b35C6F114907a02ACE07f8DfD2E409C8a65b2F",
    MATIC: "0x86b35C6F114907a02ACE07f8DfD2E409C8a65b2F",
    SOL: "8stmuD9nnrBJnhAB17hn8kZ4Zoo9kENGxu8SoHtTHKjm",
    DOGE: "D9dzH1DvZYJc9qb96Vrz9tEp2RcSpQs6LX",
    LTC: "LLv7KFCDhZx4tX23W4ViXwxCNmYjZNWqoN",
    BTC: "1DBpqUEhcX9mTHh8Mfw3jaC794kRskATA2"
};
