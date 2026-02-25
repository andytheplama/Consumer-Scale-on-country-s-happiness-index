# 🛒 Price, Happiness & Purchasing Behavior

A cross-dataset analysis exploring how product pricing affects purchasing quantity and whether national happiness scores correlate with retail consumption patterns, using the UCI Online Retail dataset and the 2025 World Happiness Report.

---

## 📌 Hypotheses

> **1.** A product's price negatively affects the quantity at which it is bought — cheaper products are ordered in higher quantities than more expensive ones.
>
> **2.** Countries with higher happiness scores exhibit different retail purchasing behavior compared to less happy countries.

---

## 📁 Datasets

| Dataset | Source | Size |
|---------|--------|------|
| `Online_Retail.xlsx` | [UCI Machine Learning Repository](https://archive.ics.uci.edu/ml/datasets/online+retail) | 541,909 transactions |
| `WHR25_Data_Figure_2_1v3.xlsx` | [World Happiness Report 2025](https://worldhappiness.report/) | 1,969 country-year records |

**Online Retail** covers transactions from a UK-based online retailer (2010–2011) across 38 countries, with fields including `InvoiceNo`, `Quantity`, `UnitPrice`, `CustomerID`, and `Country`.

**World Happiness Report** ranks countries by life evaluation score, with contributing factors including GDP per capita, social support, healthy life expectancy, freedom, generosity, and perceptions of corruption.

---

## 🔧 Tools & Libraries

| Tool | Purpose |
|------|---------|
| Python | Core language |
| Pandas | Data loading, cleaning, and merging |
| Matplotlib | Bar charts and dual-axis plots |
| Seaborn | Scatter plots |
| SciPy | Spearman correlation statistical test |

---

## 📊 Key Findings

### Hypothesis 1 — Price vs. Quantity
- After cleaning (removing negative/zero quantities and prices), **530,104 valid transactions** were analyzed
- A **Spearman correlation of -0.403** (p < 0.001) confirms a statistically significant negative relationship: lower-priced items tend to be ordered in higher quantities
- Log-scale scatter plot visualizes this inverse relationship across the full price range

### Hypothesis 2 — Happiness vs. Purchasing Behavior
- The **top 5 happiest countries** (2024 WHR): Finland, Denmark, Iceland, Sweden, Netherlands — all present in the retail dataset
- Retail purchasing volume was compared between the happiest and least happy countries with available retail data
- A dual-axis chart overlays happiness scores and total quantity ordered per country, revealing patterns in consumption relative to national well-being

---

## 📈 Visualizations

- Log-scale scatter plot: Unit Price vs. Quantity Ordered
- Bar chart: Total quantity ordered in top 5 happiest countries
- Dual-axis chart: Happiness score vs. total quantity ordered (bottom 5)
- Bar chart: Total quantity ordered in top 5 unhappiest countries

---

## 🚀 How to Run

```bash
# Clone the repository
git clone https://github.com/andytheplama/<repo-name>.git
cd <repo-name>

# Install dependencies
pip install pandas matplotlib seaborn scipy openpyxl

# Launch the notebook
jupyter notebook FTPDataScience.ipynb
```

> **Note:** Both `.xlsx` files must be in the same directory as the notebook.

---

## 📂 Repository Structure

```
FTP-DataScience/
├── FTPDataScience.ipynb
├── Online_Retail.xlsx
├── WHR25_Data_Figure_2_1v3.xlsx
└── README.md
```

---

## 👤 Author

**Andy Theplama**  
University of Arkansas — Data Science & Accounting  
[LinkedIn](https://www.linkedin.com/in/andy-theplama) · [GitHub](https://github.com/andytheplama)
