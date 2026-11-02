# ✈️ Financial Analysis — THYAO vs PGSUS

A comparative analysis of Turkish Airlines (THYAO) and Pegasus Airlines (PGSUS) based on five years of annual financial data (2020–2024). The project compares profitability, liquidity and leverage through key financial ratios, with data preparation in Excel and analysis and visualization in Python.

## 🔑 Key Findings

| Metric (2024)  | THYAO | PGSUS |
|----------------|-------|-------|
| Net Margin     | 15.1% | 11.9% |
| ROE            | 17.7% | 17.7% |
| Debt / Equity  | 0.64  | 2.14  |

- **Same return, very different risk.** In 2024 both companies delivered an identical ROE of 17.7%, but PGSUS reached it with a Debt/Equity ratio about 3.4x higher than THYAO (2.14 vs 0.64). PGSUS's return depends much more on leverage, which implies higher financial risk.
- **Different recovery paths.** Both airlines posted losses in 2020. THYAO returned to profit in 2021, while PGSUS recorded another loss that year and became profitable only in 2022.
- **A shared peak and a shared drop.** ROE peaked at around 38% for both companies in 2023 (THYAO 38.7%, PGSUS 38.2%) and fell to 17.7% in 2024, as net margins narrowed (THYAO 28.8% → 15.1%, PGSUS 29.6% → 11.9%).
- **Both deleveraged, from different starting points.** THYAO's Debt/Equity fell from 2.83 (2020) to 0.64 (2024). PGSUS peaked at 4.84 in 2021 and fell to 2.14 in 2024, but remains over three times THYAO's level.
- **THYAO liquidity improved steadily.** Its current ratio rose from 0.65 in 2020 to 1.01 in 2024.

![ROE comparison between THYAO and PGSUS](images/roe_comparison.png)

## 📊 Metrics

| Metric         | Formula                                     |
|----------------|---------------------------------------------|
| Revenue Growth | (Revenue_t / Revenue_t-1) − 1               |
| Net Margin     | Net Income / Revenue                        |
| ROE            | Net Income / Equity (year-end)              |
| Current Ratio  | Current Assets / Current Liabilities        |
| Debt / Equity  | Debt / Equity (year-end)                    |

## 🗂️ Data

- **Source:** <!-- CONFIRM --> `<e.g. annual financial statements published on KAP>`
- **Units:** <!-- CONFIRM --> THYAO figures are in USD millions; PGSUS figures are in TRY millions.
- **Debt definition:** <!-- CONFIRM --> `<e.g. financial debt only / total liabilities; whether lease liabilities are included>`
- **Inflation accounting:** <!-- CONFIRM --> `<state whether PGSUS figures are inflation-adjusted (TMS 29) or nominal>`
- `financial_ratios.csv` columns: `year, company, revenue, net_income, equity, debt, current_assets, current_liabilities, revenue_growth, net_margin, roe, current_ratio, debt_to_equity`. Ratios are stored as decimals (0.177 = 17.7%).

### Limitations

- THYAO and PGSUS are reported in different currencies, so **ratios (margin, ROE, Debt/Equity, current ratio) are comparable, but absolute amounts and revenue growth are not.** PGSUS revenue growth in TRY partly reflects high inflation in Türkiye.
- Only two companies and five years are analyzed. Findings are descriptive, not a forecast.

## 🛠️ Tools

Excel (data structuring and cleaning), Python, Pandas, Matplotlib, Jupyter Notebook, Git & GitHub

## 📁 Project Structure

```
financial-analysis-thyao-pgsus/
├── financial_analysis_thyao_pgsus.ipynb   # analysis and visualizations
├── financial_ratios.csv                   # cleaned dataset with calculated ratios
├── financial_data.xlsx                    # Excel workbook (raw data and calculations)
├── images/
│   └── roe_comparison.png
└── README.md
```

## ▶️ How to Run

```bash
git clone https://github.com/gulicin94-lgtm/financial-analysis-thyao-pgsus.git
cd financial-analysis-thyao-pgsus
pip install pandas matplotlib jupyter
jupyter notebook financial_analysis_thyao_pgsus.ipynb
```

## 👩‍💻 Author

**Güliçin Aktaş** — [LinkedIn](https://linkedin.com/in/gulicin-aktas-42b7aa160) · [GitHub](https://github.com/gulicin94-lgtm)
