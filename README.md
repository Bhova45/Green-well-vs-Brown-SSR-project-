# Green vs Ordinary: Sustainable Sharpe Ratio (SSR) Analysis

## Key Insights

- A **Green equity basket** delivers **higher returns and a higher Sharpe ratio** than an Ordinary/Brown basket over the sample, showing that sustainable investing can be competitive on traditional risk‑adjusted terms.  
- This outperformance is **regime‑dependent**: Green tends to win when climate policy momentum, ESG concern and climate news are strong, while Ordinary wins in regimes with commodity price spikes, inflation shocks or sharp rate hikes.  
- A **Sustainable Sharpe Ratio (SSR)**, which combines Sharpe with ESG/carbon metrics, **widens Green’s advantage**, highlighting which sectors offer better “sustainable value” per unit of risk.  
- For portfolio construction, **selective tilts toward high‑SSR green subsectors** (e.g., energy efficiency, transition enablers) add sustainable growth and resilience, while Ordinary assets continue to provide diversification, inflation hedging and income.

---

## Project Overview

This project compares a Green basket with an Ordinary/Brown basket across four dimensions:

1. **Return** – CAGR and cumulative performance.  
2. **Risk** – annualised volatility and maximum drawdown.  
3. **Risk‑adjusted return** – standard Sharpe ratio.  
4. **Sustainability** – ESG / carbon metrics and the derived **Sustainable Sharpe Ratio (SSR)**.

The analysis is implemented in Jupyter notebooks and uses market, macro and emissions data to study performance across different regimes.

---

## Repository Structure

- `Yahoo Finance.ipynb`  
  Downloads and cleans price data for Green and Ordinary baskets using Yahoo Finance.

- `FRED.ipynb`  
  Pulls the risk‑free rate and relevant macro series (e.g., policy rates) from FRED.

- `GHG:Carbon Emissions.ipynb`  
  Loads and cleans GHG / carbon emissions and ESG‑related data.

- `Market Risk Premium.ipynb`  
  Constructs the market risk premium and related risk factors.

- `Data Alignment and Merging.ipynb`  
  Aligns dates and merges returns, risk‑free rate, macro and carbon/ESG data into a single dataset.

- `final_notebook.ipynb`  
  End‑to‑end workflow: metrics, regime analysis, SSR computation and portfolio implications.

Key CSV files:

- `daily_returns.csv` – basket return series.  
- `rf_daily.csv` – daily risk‑free rates.  
- `ghg_macro.csv` – combined GHG and macro variables.  
- `cleaned_market_risk_premium.csv` – cleaned market premium series.  
- `aligned_data.csv` – fully aligned dataset used for analysis.  
- `basket_metrics.csv` – summary metrics for Green and Brown baskets.

---

## Methodology (High Level)

1. **Compute returns and risk metrics**  
   - Daily excess returns for Green and Ordinary baskets.  
   - Annualised return, volatility, max drawdown and Sharpe ratio.

2. **Integrate sustainability data**  
   - ESG / carbon intensity metrics at basket or sector level.  
   - Date alignment with financial series.

3. **Define Sustainable Sharpe Ratio (SSR)**  
   - Start from Sharpe and adjust using ESG / carbon metrics  
     (e.g., Sharpe divided by carbon intensity or scaled by ESG score).  
   - Compute SSR for each basket and for key subsectors.

4. **Regime analysis**  
   - Rolling 12‑month **Green – Ordinary** relative performance.  
   - Overlays of policy events, interest rates and commodity prices to identify regimes where Green vs Ordinary outperforms.



## Disclaimer

This project is for **research and educational purposes only** and does not constitute investment advice. Data sources, ESG metrics and SSR definitions are illustrative and may not capture all aspects of
