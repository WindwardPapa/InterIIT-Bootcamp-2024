# 📈 Market Neutral Mean Reversion using Dynamic Momentum Scoring

This project presents a **market-neutral long-short trading strategy** based on a **dynamic momentum ranking system**. It combines RSI and MACD signals, weighted by their **historical predictive performance**, and then further refines this signal by incorporating a **volume-based weighting mechanism**.

---

## 🔍 Overview

Rather than using traditional statistical arbitrage or cointegration, this strategy utilizes **momentum ranking signals** to construct a zero-beta portfolio. The key innovation is a **multi-level weighting system**:

- Computes **RSI** and **MACD** for a universe of stocks
- Evaluates each indicator’s **past effectiveness** in predicting returns
- Weights the indicators accordingly
- Combines them into a **momentum score**, further **weighted by a traded volume factor**
- Ranks all assets, going **long on top-ranked** and **short on bottom-ranked** securities

The strategy is designed to exploit **short-term mean-reverting opportunities** in a **market-neutral** fashion.

---

## 🛠️ Installation

Clone the repository and install dependencies:

```bash
git clone https://github.com/your-username/market-neutral-mean-reversion.git
cd market-neutral-mean-reversion
pip install -r requirements.txt
