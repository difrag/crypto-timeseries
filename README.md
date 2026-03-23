
# Crypto Alert Pipeline Project

This project demonstrates a complete pipeline for **crypto price alerting** with the following steps:

1. **Data ingestion** from the CoinGecko API
2. **Preprocessing and feature calculation** (price diff, percent change, moving averages, volatility)
3. **Crossover alert logic** (bullish / bearish based on price vs moving averages and volatility)
4. **Performance evaluation** (next-hour return, win rate, cumulative return)
5. **Analysis by market conditions** (trend & volatility)

---

## Alerts Summary

- Total alerts generated: **40**
- Mean next-hour return: **0.0003%**
- Win rate: **2.50%**

---

## Performance by Trend & Volatility

| Trend | Volatility | Count | Mean Next-Hour Return (%) | Win Rate (%) |
|-------|------------|-------|--------------------------|--------------|
| Downtrend | High Vol | 7 | 0.0000 | 0.00 |
| Downtrend | Low Vol | 7 | 0.0000 | 0.00 |
| Uptrend | High Vol | 13 | 0.0000 | 0.00 |
| Uptrend | Low Vol | 13 | 0.0011 | 7.69 |


> Note: Alert counts per group are relatively small. Metrics are illustrative and demonstrate the pipeline’s ability to segment performance by trend and volatility. For real evaluation, larger datasets or adjusted thresholds may provide more robust statistics.

---

## Plots

### Price + Moving Averages + Alerts

![Price & Alerts](plots/price_alerts.png)

### Mean Next-Hour Return by Trend & Volatility

![Return by Trend & Volatility](plots/return_by_trend_vol.png)

---

## Key Takeaways

- Alerts are generated **systematically** based on moving average crossovers and volatility conditions.
- The pipeline is fully automated from data ingestion → preprocessing → alert calculation → evaluation.
- Analysis by market conditions demonstrates **data-driven insights**, showing the best-performing conditions (e.g., uptrend + low volatility).
- This project is **portfolio-ready**: it shows both **data engineering skills** and **quantitative trading logic**.

---

*Generated automatically using Python and the processed CSV data.*
