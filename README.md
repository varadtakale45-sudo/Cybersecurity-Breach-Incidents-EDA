# Cybersecurity Breach Incidents — EDA

A beginner-friendly Exploratory Data Analysis (EDA) project on simulated cybersecurity breach data.

## 📁 Files
| File | Description |
|---|---|
| `cybersecurity_breaches.csv` | Dataset — 500 synthetic breach records (2019–2024) |
| `cybersecurity_breach_eda.ipynb` | Jupyter notebook with step-by-step analysis + explanations |

## 📊 Dataset Columns
| Column | Meaning |
|---|---|
| `incident_id` | Unique ID for the breach |
| `date`, `year`, `month`, `quarter` | When it happened |
| `industry` | Sector affected (Healthcare, Finance, etc.) |
| `breach_type` | How the attack happened (Phishing, Ransomware, etc.) |
| `attack_vector` | Entry point used (Email, Cloud, etc.) |
| `country` | Where the company is based |
| `data_sensitivity` | How sensitive the stolen data was |
| `severity` | Overall severity rating |
| `records_exposed` | Number of records leaked |
| `financial_impact_usd` | Estimated cost in USD |
| `detection_time_days` | Days taken to detect the breach |
| `resolution_time_days` | Days taken to resolve it |
| `mfa_enabled` | Was multi-factor authentication active? |
| `patch_compliance` | Was software up to date? |
| `notified_authorities` | Was the breach reported? |

## 🧠 What is EDA?
**Exploratory Data Analysis** is the process of summarizing and visualizing data to find patterns,
trends, and anomalies *before* building any model. It typically involves:
- Checking data shape, types, and missing values
- Computing summary statistics (mean, median, std)
- Visualizing distributions (histograms, bar charts, pie charts)
- Finding relationships between variables (correlation, scatter plots, box plots)

## 📓 Notebook Structure
1. Import libraries
2. Load data & inspect shape/types
3. Summary statistics
4. Industry & breach type frequency (bar charts)
5. Severity breakdown (pie chart)
6. Trend over years (line chart)
7. Financial impact distribution (histogram)
8. Severity vs. financial loss (box plot)
9. MFA effect on detection time (bar chart)
10. Correlation heatmap
11. Final summary + key takeaways

## ▶️ How to Run
```bash
pip install pandas matplotlib seaborn jupyter
jupyter notebook cybersecurity_breach_eda.ipynb
```
Run each cell top-to-bottom (`Shift + Enter`).

## 🔑 Key Concepts Explained in the Notebook
- **Mean vs Median** — average vs middle value
- **Histogram** — shows how values are spread out
- **Box plot** — shows spread + outliers across categories
- **Correlation** — measures if two numbers move together (-1 to +1)
- **Log scale** — used when data has huge outliers (e.g. financial loss)

## 📌 Key Insights
- Finance & Healthcare are the most targeted industries
- Higher severity breaches cost significantly more (often 10x+)
- MFA-enabled companies detect breaches faster on average
- Financial losses are heavily skewed — a few large breaches drive up the average

---
*Note: This dataset is synthetic (randomly generated) for learning purposes only — not real breach data.*
