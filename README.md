# Portfolio Analytics & Optimization

## Overview

This project analyzes the performance of a multi-asset portfolio compared to a benchmark (IWDA ETF), with a focus on **risk-adjusted returns**, **drawdowns**, and **portfolio optimization techniques**.

The analysis includes:

* Rolling Sharpe ratio evaluation (252-day window)
* Benchmark comparison
* Risk decomposition
* Portfolio optimization (Risk Parity & Max Sharpe)

---

## Methodology

### Key Metrics

* **Total Return**
* **CAGR (Compound Annual Growth Rate)**
* **Volatility**
* **Sharpe Ratio**
* **Rolling Sharpe Ratio (252-day)**
* **Maximum Drawdown**

### Portfolio Strategies

1. **Original Portfolio** — baseline allocation
2. **Risk Parity Portfolio** — equal risk contribution across assets
3. **Max Sharpe Portfolio** — optimized for maximum risk-adjusted return
4. **Benchmark (IWDA ETF)** — global equity benchmark

---

## Results Summary

### Original Portfolio vs Benchmark

* Lower return and Sharpe ratio than benchmark
* **Better downside protection** (lower drawdown)
* Risk is **highly concentrated**

### Risk Parity Portfolio

* Reduced volatility and drawdowns
* **Underperforms in returns and Sharpe**
* Improves diversification but still not competitive

### Max Sharpe Portfolio

* Improved return vs original portfolio
* Similar Sharpe to original
* **Higher drawdowns** → more aggressive risk profile

---

## Key Metrics

| Portfolio   | CAGR   | Volatility | Sharpe | Max Drawdown |
| ----------- | ------ | ---------- | ------ | ------------ |
| Original    | 4.99%  | 7.58%      | 0.28   | -22.45%      |
| Benchmark   | 12.05% | 14.45%     | 0.67   | -26.04%      |
| Risk Parity | 3.81%  | 5.89%      | 0.16   | -19.67%      |
| Max Sharpe  | 5.78%  | 10.39%     | 0.31   | -26.16%      |

---

## Visualizations

### Portfolio vs Benchmark

![Portfolio vs Benchmark](outputs/charts/portfolio_vs_benchmark.png)

### Rolling Sharpe Ratio (252-day)

![Rolling Sharpe](outputs/charts/rolling_sharpe_comparison.png)

### Drawdown Comparison

![Drawdown](outputs/charts/drawdown_comparison.png)

### Strategy Comparison

![Strategies](outputs/charts/strategy_comparison.png)

---

## Key Insights

* The benchmark significantly outperforms all portfolio strategies on a **risk-adjusted basis**
* The original portfolio offers **better downside protection**, but at the cost of returns
* Risk Parity improves stability but sacrifices performance
* Max Sharpe optimization increases returns but introduces **higher drawdown risk**
* All portfolios exhibit **risk concentration**, indicating potential for further diversification

---

## Future Improvements

* Add **transaction costs and rebalancing frequency**
* Include **additional asset classes** (commodities, bonds, alternatives)
* Implement **robust optimization techniques** (e.g. shrinkage, Black-Litterman)
* Perform **out-of-sample testing**
* Add **factor exposure analysis**

---

## Tech Stack

* Python (Pandas, NumPy)
* Matplotlib
* Jupyter Notebook

---

## How to Run

```bash
git clone https://github.com/FedericoGaravaglia/portfolio-analytics-python.git
cd portfolio-analytics-python
pip install pandas numpy matplotlib scipy```

Run the notebook:

```bash
jupyter notebook notebook/analysis.ipynb
```

---

## Contact

Feel free to reach out or connect if you'd like to discuss portfolio construction, quantitative finance, or this project.
