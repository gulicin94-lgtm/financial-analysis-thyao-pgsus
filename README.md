# ✈️ Financial Analysis — THYAO vs PGSUS

A comparative analysis of Turkish Airlines (THYAO) and Pegasus Airlines (PGSUS) based on five years of financial statement data . The project compares profitability, liquidity and leverage using key financial ratios, with data preparation in Excel and analysis and visualization in Python.

## 🔑 Key Findings

| Metric (2024)        | THYAO | PGSUS |
|----------------------|-------|-------|
| ROE                  | ~18%  | ~18%  |
| Debt / Equity        | 0.64  | 2.14  |

- **Similar return, very different risk.** In 2024 both companies reached a similar ROE (~18%), but PGSUS did so with a Debt/Equity ratio about 3.3x higher than THYAO (2.14 vs 0.64). PGSUS's return relies much more on leverage, which implies higher financial risk.
- **Different recovery paths.** THYAO returned to profit in 2021, while PGSUS continued to report a net loss that year.

![ROE comparison between THYAO and PGSUS](images/roe_comparison.png)

## 📊 Metrics Analyzed

| Metric            | Formula                               |
|-------------------|---------------------------------------|
| Revenue Growth    | (Revenue_t − Revenue_t−1) / Revenue_t−1 |
| Net Margin        | Net Income / Revenue                  |
| ROE               | Net Income / Equity                   |
| Current Ratio     | Current Assets / Current Liabilities  |
| Debt / Equity     | `<Debt definition>` / Equity          |

## 🗂️ Data

- **Source:** `<e.g. annual financial statements published on KAP (Public Disclosure Platform)>`
- **Currency and units:** `<e.g. TL, in thousands>`
- **Inflation accounting:** `<state whether figures are inflation-adjusted (TMS 29) or nominal, and how that may affect comparability across years>`
- **Debt definition:** `<e.g. total liabilities, or financial debt only; state whether lease liabilities are included>`
- **Limitations:** Only two companies and five years are analyzed, so findings are descriptive and should not be read as a forecast.

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
