# 🧠 ULTIMATE AI STOCK ANALYSIS PROMPT — “PETER LYNCH + INSTITUTIONAL STRATEGY + FUTURE SCENARIOS”

---

## 🎯 OBJECTIVE

Act as the **Head of Equity Research** at a **top-tier sell-side or buy-side investment firm** serving institutional clients.  
Your mission: produce a **complete, audit-grade, evidence-based equity research report** that applies **Peter Lynch’s 8 investing rules** while integrating quantitative backtesting, valuation modeling, technical trend analysis, and future scenario forecasting.

The report must be **data-first, defensible, timestamped, and presentation-ready**.

Deliver all outputs **in this single response**:
- Executive summary (≤5 bullets)
- One-page memo (slide-ready)
- Full 5–12 page research report (markdown)
- Historical performance & trend analysis
- Quantitative backtests vs. benchmark (1/3/5/10/15 years)
- DCF, peer-relative, and multi-scenario valuation models
- Quality, risk, and consistency scores
- Future scenarios (Bear / Base / Bull)
- Buy/Hold/Sell recommendation with conviction levels
- Position sizing (concentrated, diversified, institutional)
- JSON summary
- PNG charts (total return, trend, DCF, score bar)
- CSV summary of key data
- Source list + timestamps

---

## 📜 PETER LYNCH INVESTING FRAMEWORK

Explicitly apply these in a “Lynch Checklist” section with quotes and evidence:

1. **Edge:** Use what you already know; identify investor edge.  
2. **Contrarian:** Ignore the herd; explain consensus bias.  
3. **Fundamentals > Stock:** Long-term stock = company performance; compare both.  
4. **Focus:** Follow only what you can manage; evaluate coverage capacity.  
5. **Financials:** Never invest without checking solvency; show liquidity, leverage, Z-score.  
6. **Avoid Hype:** Prefer great firms in dull industries; flag overheated sectors.  
7. **Recovery:** If the industry is troubled, pick the survivors; show revival indicators.  
8. **Concentration:** A few big winners drive results; suggest ideal position sizing.

---

## 🧾 REQUIRED DATA INPUTS

Use the latest available data. Timestamp everything (UTC).

**Company Fundamentals**
- Ticker, Exchange, CUSIP, CIK
- Current Price, Market Cap, Shares Outstanding
- Segment & geographic revenue mix
- 10 years of financial statements (IS, BS, CF)
- Growth metrics: Revenue, EBIT, EPS, FCF CAGR (1/3/5/10y)
- Margins: Gross, Operating, Net, FCF
- Leverage: Total Debt, Net Debt/EBITDA, Interest Coverage
- Liquidity: Current & Quick Ratios
- ROE, ROIC, ROA
- Insider & institutional ownership, buyback/dilution trends
- Analyst consensus (EPS forecast, PT, sentiment)
- Short interest, beta, volatility

**Historical & Technical**
- Daily total return data (≥10 years preferred)
- Benchmark (S&P 500 or relevant)
- Technical trends: 50/200-day MA, RSI, MACD, volatility %
- Recent momentum: +1m, +3m, +6m, +1y performance
- Price channel (support/resistance zones)
- Relative strength vs benchmark
- Volume & accumulation trend

**Macro & Sector**
- Industry growth rate
- Key macro drivers
- Commodity, regulatory, or FX exposure
- Sector performance comparison

---

## ⚙️ ANALYTICAL TASKS

### 1. 📈 Historical Performance
- Compute total return CAGR (1/3/5/10/15y)
- Rolling 12m / 36m excess returns
- CAPM Alpha, Beta, t-stats, Sharpe, Sortino, Max Drawdown
- Statistical significance (bootstrap p-value)
- Consistency Index: % of rolling 3y windows beating benchmark >2%/yr

### 2. 📊 Technical Trend & Price Momentum
- Identify trend (Uptrend / Downtrend / Sideways)
- Compare 50MA vs 200MA for crossover
- RSI range (overbought/oversold zones)
- MACD signal (bullish/bearish divergence)
- Short-term volatility % vs historical average
- Recent price action summary (1m, 3m, 6m, 12m return vs index)

### 3. 💎 Quality & Consistency Score (0–100)
| Factor | Weight | Description |
|---------|---------|-------------|
| ROIC Stability | 8% | Standard deviation over 10y |
| FCF Conversion | 7% | FCF/Net Income |
| Margin Stability | 5% | Std. dev. of margins |
| Piotroski F-Score | 5% | Financial strength |
| Balance Sheet Strength | 5% | Leverage & liquidity |
| Capital Allocation | 5% | Buybacks, dividends, reinvestment quality |

### 4. 💰 Valuation Models
Perform:
- **Discounted Cash Flow (DCF)** (10y explicit + terminal via both Gordon & exit multiple)
- **Peer-relative multiples** (EV/EBITDA, P/E, PEG, P/FCF)
- **Scenario Analysis:**
  - **Bear Case:** pessimistic growth, high WACC, multiple contraction
  - **Base Case:** realistic consensus growth & normalized margins
  - **Bull Case:** optimistic revenue growth, margin expansion, re-rating
  - Output: fair value range with probability weights

### 5. 🧠 Moat & Strategic Durability
Rate each 0–5 (None → Enduring):
1. Network Effects  
2. Switching Costs  
3. Scale Advantages  
4. IP/Brand/Regulation  
5. Cost Leadership  
→ Aggregate to Moat Rating

### 6. ⚠️ Risk Matrix
Top 10 risks table:
| Risk | Probability % | NAV Impact % | Description |
|------|----------------|---------------|--------------|

### 7. 🚀 Catalysts
Time-based list of near/mid/long-term drivers:
| Term | Catalyst | Confidence | Expected Impact |
|------|-----------|-------------|----------------|

### 8. 📦 Position Sizing
| Portfolio Type | Recommended Weight | Rationale |
|----------------|--------------------|------------|
| 5-Stock Concentrated | X% | Based on conviction and upside |
| 20-Stock Diversified | X% | Risk-adjusted sizing |
| Institutional Block | USD size, expected impact, trade horizon |

### 9. 🧾 Governance & ESG
Rate (1–5): Board independence, CEO alignment, transparency, ESG controversies.

---

## 🔮 FUTURE SCENARIOS & RECOMMENDATION

Include this dedicated section:

### 🔭 Scenario Modeling
| Scenario | Growth Assumption | Valuation Multiple | Fair Value | Upside/Downside % | Probability |
|-----------|------------------|--------------------|-------------|-------------------|--------------|
| Bear | Slow growth, margin compression | Low multiple | $X | -Y% | 25% |
| Base | Consensus trajectory | Market average | $X | +Y% | 50% |
| Bull | Strong growth, margin expansion | Premium multiple | $X | +Z% | 25% |

### 💡 Final Recommendation
Provide:
- **Buy / Hold / Sell** recommendation
- **Conviction Level** (High / Medium / Low)
- **12m, 24m, 36m Target Prices**
- **Expected Returns** and Confidence Intervals
- **Narrative Summary:** why the stock fits (or doesn’t) a Peter Lynch approach
- **Position Sizing Guidance:** per portfolio type

---

## 📊 SCORING MODEL (Weights)

| Metric | Weight |
|--------|---------|
| Historical Outperformance | 30% |
| Quality & Consistency | 25% |
| Valuation Attractiveness | 20% |
| Moat & Durability | 15% |
| Governance & Liquidity | 10% |

Final **Composite Score (0–100)** = weighted sum.  
Also compute **Confidence Band (High/Med/Low)** and **Trend Direction**.

---

## 🧮 FORMULAS (show all in report)

- CAGR = (End / Start)^(1/n) − 1  
- FCF = CFO − CapEx  
- ROIC = NOPAT / Invested Capital  
- WACC = rf + β × ERP + (Debt% × After-tax Cost of Debt)  
- Alpha = r_stock − [rf + β × (r_market − rf)]  
- Altman Z, Piotroski F, Beneish M formulas (explicit)

---

## 💾 JSON OUTPUT SCHEMA

```json
{
  "ticker":"TICKER",
  "as_of":"YYYY-MM-DDTHH:MM:SSZ",
  "price":0.0,
  "market_cap":0.0,
  "trend_analysis":{
    "trend":"Uptrend|Downtrend|Sideways",
    "momentum_1m_pct":0.0,
    "momentum_3m_pct":0.0,
    "momentum_6m_pct":0.0,
    "momentum_12m_pct":0.0,
    "rsi":0.0,
    "macd_signal":"Bullish|Bearish|Neutral"
  },
  "recommendation":{
    "rating":"Strong Buy|Buy|Hold|Trim|Sell|Strong Sell",
    "conviction":"High|Medium|Low",
    "target_price":{"12m":0.0,"24m":0.0,"36m":0.0},
    "expected_return":{"12m_pct":0.0,"24m_pct":0.0,"36m_pct":0.0}
  },
  "future_scenarios":[
    {"scenario":"Bear","growth":"Low","fair_value":0.0,"upside_pct":0.0,"probability_pct":25},
    {"scenario":"Base","growth":"Normal","fair_value":0.0,"upside_pct":0.0,"probability_pct":50},
    {"scenario":"Bull","growth":"High","fair_value":0.0,"upside_pct":0.0,"probability_pct":25}
  ],
  "composite_score":0.0,
  "component_scores":{
    "outperformance":0.0,
    "quality":0.0,
    "valuation":0.0,
    "moat":0.0,
    "governance":0.0
  },
  "moat_rating":"None|Weak|Moderate|Strong|Enduring",
  "top_risks":[{"risk":"","probability_pct":0.0,"impact_pct_nav":0.0}],
  "position_size":{
    "concentrated_5":{"percent_portfolio":0.0},
    "diversified_20":{"percent_portfolio":0.0},
    "institutional_block":{"usd_size":0.0,"trade_horizon_days":0}
  },
  "sources":[{"name":"","url":"","retrieved":"YYYY-MM-DDTHH:MM:SSZ"}]
}
