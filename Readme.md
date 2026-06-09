# Options Portfolio Optimization & Risk Analytics

# Project - Kotak Mahindra

# Overview
This repository contains a quantitative risk assessment and derivatives pricing engine built in Python. The project simulates a professional advisory engagement, focusing on structuring a multi-leg options portfolio and executing dynamic delta-gamma hedging strategies to mitigate tail-risk under market volatility.

# Key Features
* **Quantitative Risk Assessment:** Processed ~60 trading days of historical NSE market data to extract return statistics (annualized volatility, skewness, and kurtosis) and map non-Gaussian tail risks.
* **Derivatives Pricing Engine:** Developed a Black-Scholes-Merton (BSM) pricing model to evaluate 30 unique option contracts (5 strikes × 3 maturities × calls/puts).
* **Volatility Surface Construction:** Computed implied volatilities from market prices to construct a 3D volatility surface, enabling market-aligned sensitivity analysis.
* **Dynamic Hedging & VaR Simulation:** Engineered a delta-gamma neutral multi-leg portfolio, successfully simulating portfolio PnL under ±1% and ±2% stock price shocks.

# Business Impact
* Slashed directional market exposure (Delta) from **-1.097** to **-0.223** and neutralized Gamma to **0.000**.
* Achieved a **~99.98% reduction in 95% Historical VaR** (from 21.95 to 0.0035).
* Achieved a **~99.98% reduction in 99% Parametric VaR** (from 30.69 to 0.0048).
* Reduced overall PnL sensitivity under ±2% underlying price shocks by **~80%**, demonstrating institutional-grade risk mitigation.

# Tech Stack
* **Language:** Python
* **Libraries:** `pandas`, `numpy`, `scipy` (statistical distributions and optimization), `yfinance` (API data extraction), `matplotlib` (3D surface plotting).

# Repository Structure
* `/notebooks`: Contains the primary Jupyter Notebook with the step-by-step mathematical implementation, BSM functions, Greeks calculations, and VaR backtesting.
* `/data`: (Placeholder) Directory for historical NSE pricing datasets.

# How to Run
1. Clone this repository: `git clone https://github.com/yourusername/kotak-derivatives-risk-engine.git`
2. Install the required dependencies: `pip install -r requirements.txt`
3. Run the Jupyter Notebook in the `/notebooks` directory.
