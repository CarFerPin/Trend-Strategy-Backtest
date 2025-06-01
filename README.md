## 🧾 **Can We Make Money with This Strategy?**

We've developed and evaluated a **trend-following trading strategy**, using a robust backtesting pipeline to quickly assess its performance across diverse stocks and varying market conditions. Our goal was to see if this strategy holds potential for profitability.

The strategy was first tested over a **6-month period** using **1-hour candles** across **55 different stocks**. This initial batch of backtests provided encouraging insights: over **55% of the analyzed stocks delivered positive returns**, with a standout high return of **45.6%**. The minimum return observed was a contained **-7.5%**, leading to an **average total return of 2.9%** across all backtests. While the maximum drawdown reached **19%**, the **mean drawdown was a well-contained 6.9%** over the analyzed period. These results offer **promising evidence of the strategy's potential viability**.

---

### ✅ Strategy Quality Summary (6-Month Period):

* **Positive Performance:**
    * **31 out of 55** backtests (56.4%) delivered a **positive total return**.
    * **31 out of 55** backtests (56.4%) showed a **positive expectancy**.
    * **8 out of 55** backtests (14.5%) achieved a **Sharpe Ratio greater than 1.0**, indicating strong risk-adjusted returns.

* **Return Metrics:**
    * The **average total return** across all 55 backtests was **2.9%**.
    * The **maximum total return** achieved in any single backtest was an impressive **45.6%**.
    * The **minimum total return** observed was **-7.52%**.

* **Risk Metrics:**
    * The **maximum drawdown** encountered was **18.56%**.
    * The **average drawdown** across all backtests was **6.86%**.

---


We found similar results when the strategy was extended and tested over a **1-year period** using **4-hour candles** (a second batch of 55 backtests) with more than 60% of them producing positive returns but with more volatility and larger downside risk, which is consistent for the larger period of time and the larger return achieved. This suggests the strategy is hitting stability over time and across risk-return scenarios. While these specific findings aren't detailed here due to space, they are easily reproducible by simply adjusting the `yfinance` data feeder parameters. Here's a summary of the quality results for this second batch of backtests:


---

### ✅ Strategy Quality Summary (1-Year Period):

* **Positive Performance:**
    * **34 out of 55** backtests (61.8%) delivered a **positive total return**.
    * **34 out of 55** backtests (61.8%) showed a **positive expectancy**.
    * **13 out of 55** backtests (23.6%) achieved a **Sharpe Ratio greater than 1.0**, indicating strong risk-adjusted returns.

* **Return Metrics:**
    * The **average total return** across all 55 backtests was **5.15%**.
    * The **maximum total return** achieved in any single backtest was an impressive **90.43%**.
    * The **minimum total return** observed was **-13.34%**.

* **Risk Metrics:**
    * The **maximum drawdown** encountered was **36.12%**.
    * The **average drawdown** across all backtests was **9.3%**.

---

## But—**is this strategy ready for live trading? Absolutely not.**

What we have is a solid **initial prototype** that clearly demonstrates the strategy's feasibility. Before it can be considered for production, significant refinement is still needed. This includes:

* **Robust statistical filtering:** Implementing more rigorous tests to ensure the observed performance isn't just due to random chance.
* **Parameter tuning and walk-forward validation:** Optimizing the strategy's settings and rigorously validating them on unseen data to prevent overfitting.
* Potential integration of **machine learning or deep learning** techniques to further optimize signal generation and filtering.
* **Code cleanup and modularization:** Making the code more organized and easier to maintain for correct engineering before production.

Nevertheless, these results represent a strong **first step**. With further development, this strategy framework could evolve into a powerful, systematic trading tool.
```
