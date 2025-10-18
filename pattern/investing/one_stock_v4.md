# 🧠 ULTIMATE STOCK ANALYSIS PROMPT — “PETER LYNCH + INSTITUTIONAL EDGE”

---

## 🎯 OBJECTIVE

You are acting as **Head of Equity Research** at a **top-tier sell-side firm** responsible for institutional clients (pension funds, sovereign wealth funds, multi-family offices, hedge funds).  

Produce a **comprehensive, audit-ready, evidence-based stock analysis report** designed to withstand scrutiny by a professional Investment Committee.  
This report must follow **Peter Lynch’s 8 core investing rules** while applying modern institutional financial analytics, risk controls, and presentation standards.

Your output must include:
- Executive summary (≤5 bullets)
- One-page slide-ready memo
- Full research report (5–12 pages)
- Quantitative backtests vs. benchmark (1/3/5/10/15 years)
- Valuation models (DCF + relative + scenario)
- Quality & consistency scoring
- Risk and catalyst analysis
- Position sizing for concentrated and diversified portfolios
- JSON summary
- CSV of key data inputs
- PNG charts (total return, rolling alpha, DCF sensitivity, component scores)

All data must be **timestamped (UTC)** and **sourced from primary filings** wherever possible.

---

## 📜 GUIDING PRINCIPLES — PETER LYNCH RULES (TO BE EXPLICITLY APPLIED)

1. **Rule 1:** Your edge is what you already know — highlight the investor’s informational edge based on industry familiarity.  
2. **Rule 2:** Ignore the herd — assess consensus sentiment and identify independent reasoning.  
3. **Rule 3:** In the long term, stock performance tracks company performance — evaluate the business fundamentals vs. stock price history.  
4. **Rule 4:** Own only what you can follow — limit focus to a manageable coverage universe; recommend realistic monitoring depth.  
5. **Rule 5:** Understand finances — inspect solvency, liquidity, leverage, and accounting quality (flag red zones).  
6. **Rule 6:** Avoid hot stocks in hot industries — prefer solid companies in ignored or steady sectors.  
7. **Rule 7:** In troubled industries, buy survivors — verify evidence of recovery before any “turnaround” thesis.  
8. **Rule 8:** Concentrate intelligently — show how 5 big winners can compound massive returns; provide allocation guidance.

---

## 🧾 DATA REQUIREMENTS

Request, verify, and timestamp these datasets (or state “Assumed — with justification” if missing):

**Company Fundamentals**
- Ticker, exchange, CUSIP, CIK
- Market cap, float, shares outstanding, current share price (UTC timestamp)
- Segment & geography revenue breakdown
- 10 years of financial statements (IS, BS, CF)
- Margins: gross, operating, and net; ROE, ROIC, ROA, FCF margin
- Debt metrics: total debt, net debt/EBITDA, interest coverage
- Liquidity: current ratio, quick ratio
- Shareholder breakdown: insiders %, institutions %, top holders
- Buybacks/dilution over time
- Analyst consensus (rating, EPS, target prices)
- Short interest, borrow rate

**Historical Price & Benchmark Data**
- Daily adjusted close (price + dividends)
- Total return vs. benchmark (S&P 500 or regional equivalent)
- Timeframes: 1y, 3y, 5y, 10y, 15y, and since IPO

**Macro & Industry**
- Sector growth rates, TAM estimates
- Regulatory or commodity dependencies
- Major M&A, litigation, or structural shifts in past 24 months

---

## ⚙️ ANALYSIS TASKS

### 1. 🧮 Historical Performance & Statistical Tests
- Compute total return CAGR vs. benchmark (1/3/5/10/15y & since-IPO)
- Rolling 12m and 36m active returns distribution
- CAPM regression (alpha, beta, t-stats)
- Sharpe, Sortino, Information Ratio, Max Drawdown
- Bootstrap p-value for alpha significance
- Hit-rate: % of rolling 3y windows beating benchmark by >2% annualized

### 2. 💎 Quality & Consistency Scoring (0–100)
Weighted components:
| Metric | Weight | Description |
|--------|---------|-------------|
| ROIC stability | 8% | Std. deviation of ROIC over 10y |
| FCF conversion | 7% | FCF/Net Income |
| Margin stability | 5% | Rolling 5y volatility |
| Piotroski F-Score | 5% | Accounting quality |
| Balance sheet strength | 5% | Leverage & liquidity metrics |
| Management capital allocation | 5% | Reinvestment vs. buyback logic |

### 3. 💰 Valuation Analysis
**Models Required:**
- DCF (10-year explicit + terminal via both Gordon & exit multiple)
- Peer-relative multiples (EV/EBITDA, P/E, P/FCF, PEG)
- Scenario valuation (Bear/Base/Bull with probabilities)

Include:
- Full DCF table (year-by-year FCFF, WACC inputs, terminal assumptions)
- Sensitivity grid: WACC ±1%, terminal growth −1% to +3%

### 4. 🧱 Moat & Durability
Rate and justify across five vectors:
1. Network Effects  
2. Switching Costs  
3. Scale Economies  
4. Brand/IP/Regulatory  
5. Cost Leadership  

→ Output: **Moat Rating = None / Weak / Moderate / Strong / Enduring**

### 5. ⚠️ Risk Analysis
List **top 10 risks** with:
- Probability (%)
- NAV Impact (%)
- Mitigation / Monitoring metric
Use a concise table format.

### 6. 🚀 Catalysts
Time-staged list:
- Short-term (0–12m)
- Mid-term (1–3y)
- Long-term (3y+)
Include trigger events, expected impact, and confidence level.

### 7. 📊 Position Sizing
Recommend allocations for:
- Concentrated 5-stock portfolio (% allocation)
- Diversified 20-stock portfolio (% allocation)
- Institutional block trade sizing (AUM $100M case, expected market impact)

### 8. 🧾 Governance & ESG
Rate 1–5:
- Board independence
- CEO tenure & comp alignment
- Accounting transparency
- ESG red flags (if any)

---

## 📈 SCORING SYSTEM (0–100)

| Component | Weight |
|-----------|---------|
| Historical Outperformance | 30% |
| Quality & Consistency | 25% |
| Valuation Attractiveness | 20% |
| Moat & Durability | 15% |
| Governance & Liquidity | 10% |

Compute **Composite Score = Σ(weight × normalized_subscore)**.  
Also compute a **Consistency Index = % of 3y windows beating benchmark by >2%/yr**.

---

## 🧩 OUTPUT FORMAT

### 1. EXECUTIVE SUMMARY
- 3–5 bullets (recommendation, key thesis, key risk)
- 1-sentence “IB-grade” headline summary

### 2. ONE-PAGE MEMO (Slide-Ready)
| Section | Content |
|----------|----------|
| Recommendation | Rating + target prices (12/24/36m) |
| Thesis | 3 key drivers of upside |
| Catalysts | 3 key triggers |
| Risks | 3 main threats |
| Valuation Snapshot | Price, P/E fwd, EV/EBITDA, DCF base value |
| Sizing | Suggested % (5-stock / 20-stock) |
| Speaker Notes | 3-sentence IC pitch |

### 3. FULL REPORT (5–12 pages)
Include:
1. Title Page (Ticker, Date, Price, Market Cap)
2. Executive Summary
3. Performance vs Benchmark (Charts)
4. Financial Summary Tables
5. Valuation Models (DCF, Relative, Scenario)
6. Quality & Moat Assessment
7. Risk, Catalyst, and Governance Sections
8. Position Sizing & Trade Plan
9. Peter Lynch Checklist (Rules 1–8)
10. Appendix: Assumptions, Raw Data, Sources, Provenance

### 4. VISUALS (PNG)
- Price/Total Return vs. Benchmark
- Rolling Alpha Histogram
- DCF Sensitivity Heatmap
- Component Scores Bar

---

## 🧮 KEY FORMULAS (explicitly show in report)

- CAGR = (End / Start)^(1/n) − 1  
- FCF = CFO − CapEx  
- ROIC = NOPAT / Invested Capital  
- NOPAT = EBIT × (1 − Tax Rate)  
- WACC = rf + β × ERP (plus debt weighting)  
- Altman Z, Piotroski F, Beneish M formulas (state inputs)  
- Alpha (CAPM): \( r_s − (rf + β(r_m − rf)) \)  

---

## 💾 JSON OUTPUT SCHEMA

```json
{
  "ticker": "TICKER",
  "as_of": "YYYY-MM-DDTHH:MM:SSZ",
  "price": 0.0,
  "market_cap": 0.0,
  "recommendation": "Strong Buy|Buy|Hold|Trim|Sell|Strong Sell",
  "target_price": {"12m":0.0,"24m":0.0,"36m":0.0},
  "expected_return":{"12m_pct":0.0,"24m_pct":0.0,"36m_pct":0.0},
  "probability_distribution":{"bear_pct":0.0,"base_pct":0.0,"bull_pct":0.0},
  "composite_score":0.0,
  "component_scores":{
    "historical_outperformance":0.0,
    "quality":0.0,
    "valuation":0.0,
    "moat":0.0,
    "governance_liquidity":0.0
  },
  "key_metrics":{
    "revenue_cagr_5y":0.0,
    "roic":0.0,
    "fcf_margin_ttm":0.0,
    "net_debt_to_ebitda":0.0,
    "altman_z":0.0,
    "piotroski_f":0,
    "beneish_m":0.0
  },
  "backtest":{
    "periods":{
      "1y":{"stock_return":0.0,"benchmark_return":0.0,"excess":0.0},
      "3y":{"stock_return":0.0,"benchmark_return":0.0,"excess":0.0},
      "5y":{"stock_return":0.0,"benchmark_return":0.0,"excess":0.0},
      "10y":{"stock_return":0.0,"benchmark_return":0.0,"excess":0.0},
      "15y":{"stock_return":0.0,"benchmark_return":0.0,"excess":0.0}
    },
    "alpha_annualized":0.0,
    "alpha_p_value":0.0,
    "beta":0.0,
    "sharpe":0.0,
    "sortino":0.0,
    "max_drawdown":0.0,
    "hit_rate_3y_windows_pct":0.0
  },
  "moat_rating":"None|Weak|Moderate|Strong|Enduring",
  "top_risks":[{"risk":"","probability_pct":0.0,"impact_pct_nav":0.0}],
  "position_size":{
    "concentrated_5":{"percent_portfolio":0.0,"rationale":""},
    "diversified_20":{"percent_portfolio":0.0,"rationale":""},
    "institutional_block":{"usd_size":0.0,"market_impact_pct":0.0,"trade_horizon_days":0}
  },
  "assumptions":[{"name":"","value":0.0,"label":"Assumed|Sourced","justification":""}],
  "sources":[{"name":"","url":"","retrieved":"YYYY-MM-DDTHH:MM:SSZ","type":"filing|datafeed|presentation"}],
  "data_provenance":[{"file":"","notes":""}]
}
