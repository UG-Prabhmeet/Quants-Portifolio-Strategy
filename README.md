# Quants-Portfolio-Strategy

A sophisticated quantitative trading strategy designed to maximize the **Sharpe Ratio** while operating under real-world trading constraints. This project implements a backtesting engine to evaluate the performance of a portfolio rebalancing strategy across multiple assets.

## 🚀 Overview

This strategy was developed for the **Quants Hackathon 2025**. It uses a dynamic allocation approach based on historical Sharpe Ratios to decide whether to go long or short on various stocks, while strictly adhering to exposure limits.

### Key Features
- **Sharpe Ratio Optimization**: Dynamically ranks assets based on risk-adjusted returns.
- **Exposure Control**: Ensures net exposure remains within 10% and individual asset weights are capped at 5%.
- **Realistic Backtesting**: Accounts for **commission (0.05%)** and **slippage (0.03%)**.
- **Automated Rebalancing**: Supports monthly or weekly rebalancing frequencies.
- **Negative NAV Protection**: Built-in safeguards to prevent the portfolio value from dropping below zero.

## 🛠️ Requirements

To run this project, you need:
- Python 3.x
- Pandas
- NumPy

Install dependencies via pip:
```bash
pip install pandas numpy datetime
```

## 📂 Project Structure

- `2022UCM2305.py`: The main trading strategy script.
- `Prices.csv`: Historical pricing data for the assets (Required for execution).
- `README.md`: Project overview and setup instructions.

## 📈 How to Run

1. Ensure `Prices.csv` is in the same directory (or update the path in the script).
2. Run the strategy script:
   ```bash
   python 2022UCM2305.py
   ```
3. The script will output the **Annualized Sharpe Ratio** upon completion.

---
*Developed for Quants Hackathon 2025.*
