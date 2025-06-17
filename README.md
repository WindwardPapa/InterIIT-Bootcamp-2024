## Inter IIT Bootcamp 2024
# 📈 Market Neutral Mean Reversion using Dynamic Momentum Scoring

This project presents a **market-neutral long-short trading strategy** based on a **dynamic momentum ranking system**. It combines RSI and MACD signals, weighted by their **historical predictive performance**, and then further refines this signal using a **volume-based weighting mechanism**.

## 🔍 Overview

Instead of using traditional statistical arbitrage (like cointegration), this strategy adopts a **signal-based momentum approach**:

- Calculates **RSI** and **MACD** for a set of equities
- Evaluates each indicator's **predictive strength based on historical returns**
- Combines these indicators with **dynamic weights**
- Applies a second layer of weighting using **traded volume as a confidence metric**
- Ranks all stocks by their final score
- Builds a **market-neutral portfolio** by taking **long positions** on the top-ranked and **short positions** on the bottom-ranked stocks

---

## 🛠️ Installation

Clone the repository and install dependencies:

```bash
git clone https://github.com/WindwardPapa/InterIIT-Bootcamp-2024.git
cd InterIIT-Bootcamp-2024
pip install -r requirements.txt
