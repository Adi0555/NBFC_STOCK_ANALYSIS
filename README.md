# NBFC - Bajaj Finserv, Cholamandalam Finance, and Jio Finance

## Project Overview
This repository serves as a systematic approach to technical analysis and performance tracking within the Non-Banking Financial Company (NBFC) sector.
The project integrates **technical indicator signals** (RSI and Moving Averages) to build a comprehensive view of portfolio health and trading efficiency.
Designed as an analytical framework, this project demonstrates the workflow of identifying market trends,
executing trades based on those signals, and auditing the realized financial outcomes.

## Project Architecture
The analysis is segmented into three core data components:
### 1. Technical Signal Analysis (`RSI_&_MA.csv`)
This file acts as the "Decision Engine." It evaluates the market health of key NBFC stocks (e.g., Bajaj Finserv, Jio Financial Services, Chola Financial Holdings) using established quantitative metrics:
* **Momentum Metrics:** Tracks the **Relative Strength Index (RSI)** to identify overbought (>70) and oversold (<30) conditions.
* **Trend Dynamics:** Calculates **Simple Moving Averages (SMA)** across multiple time horizons (5, 20, 50, and 200 days) to identify support, resistance, and potential trend reversals.

### 2. Trade Execution Log (`Trade Log.csv`)
This including the Trade log of Stock Market form 14 Oct 2025 to 23 Oct 2025 . It captures the real-world application of technical signals:
* **Lifecycle Tracking:** Records the entry date, exit date, volume, and pricing for each transaction.
* **P&L Calculation:** Computes the delta between *Amount Invested* and *Amount Received*,
  providing a clear view of realized profit or loss per trade.
* **Execution Efficiency:** Allows for post-trade analysis to determine if entry/exit timings aligned with the technical signals generated in the first file.

### 3. Portfolio Summary (`PortFolio Return.csv`)
This file consolidates the raw data into high-level business intelligence:
* **Performance Aggregation:** Calculates net returns, total capital exposure, and sector-specific performance metrics.
* **Strategy Evaluation:** Compares the theoretical effectiveness of the technical strategy against the actual realized financial return of the portfolio.

## 💡 Methodology
The workflow follows a standard financial analytics lifecycle:
1.  **Signal Generation:** Identifying entry/exit points using Moving Average crossovers and RSI divergence.
2.  **Trade Execution:** Mapping these signals to historical buy/sell orders.
3.  **Performance Auditing:** Calculating net returns and summarizing portfolio exposure to refine future trading strategies.
