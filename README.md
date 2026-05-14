# Superstore-EDA
# 🛒 Superstore Sales & Profitability Analysis

A data analytics project exploring what actually drives profit — and what destroys it — across a US retail superstore's four years of sales data.

---

## 🚀 Key Takeaways

- Discovered that **orders with discounts above 20% are loss-making on average** — confirmed through statistical analysis
- Found that **Tables and Bookcases lose money every year** despite generating consistent sales revenue
- Identified a **reliable Q4 seasonality spike** repeating across all four years — a pattern the business can plan around
- Revealed that the **Central region's underperformance is a margin problem, not a demand problem**
- Delivered insights through **Python-based visualizations** including correlation heatmaps, trend charts, and regional profit breakdowns

---

## 📊 Dashboard & Visual Analysis

<img width="867" height="634" alt="Screenshot 2026-05-14 at 2 44 41 PM" src="https://github.com/user-attachments/assets/df7aad8e-030f-45d3-a866-e48dfcfe599f" />

<img width="942" height="377" alt="Screenshot 2026-05-14 at 2 45 13 PM" src="https://github.com/user-attachments/assets/8db33edf-9c80-4610-b86a-64bb63c225ad" />

<img width="937" height="349" alt="Screenshot 2026-05-14 at 2 45 45 PM" src="https://github.com/user-attachments/assets/bdbfde44-6b7e-421b-aea1-eee1303b1ddc" />

<img width="946" height="334" alt="Screenshot 2026-05-14 at 2 47 01 PM" src="https://github.com/user-attachments/assets/3348afb9-ab5c-4689-96be-67b18165be11" />

---

## 📌 Problem

Retail businesses often focus on growing sales — but high sales don't always mean high profit. This project investigates a more important question:

> *Where is the business actually making money, and where is it quietly losing it?*

Using four years of order-level data across products, regions, and discount tiers, this analysis identifies the specific categories, sub-categories, and behaviours that drive or destroy profitability — and translates those findings into concrete business recommendations.

---

## 🧠 Approach

### 1. Data Cleaning & Validation

- Checked for missing values, duplicate rows, and formatting inconsistencies
- Parsed date columns to enable time-based analysis
- Validated numeric ranges to confirm negative profit rows were real loss-making orders, not data errors
- Created derived columns including Profit Margin and Order Month for deeper analysis

### 2. Exploratory Analysis

Analysed the data across four dimensions:

| Dimension | What It Examines |
| --- | --- |
| Univariate Analysis | Distribution of Sales, Profit, and Discount individually |
| Bivariate Analysis | Relationships between variables — especially discount vs profit |
| Regional & Category Analysis | Which regions and product types are profitable vs loss-making |
| Time Series Analysis | Monthly trends, seasonality patterns, and year-over-year growth |

### 3. Statistical Validation

- Applied **linear regression** to measure the relationship between discount rate and profit
- Used **Pearson correlation** and **p-value testing** to confirm findings are statistically significant and not random chance
- Grouped discounts into bands to pinpoint the exact threshold where orders become loss-making

---

## 📈 Key Insights

- **Discounting above 20% destroys profit** — the correlation between discount and profit is statistically significant (Pearson r = −0.22, p < 0.001). Orders above the 20% threshold are loss-making on average
- **Tables and Bookcases are structurally loss-making** — across all four years, these sub-categories generated revenue but produced negative total profit, pointing to a pricing and cost structure problem
- **Technology is the most profitable category** — highest profit margin despite moderate order volume, led by Phones and Copiers
- **Q4 drives a consistent seasonal spike every year** — November and December reliably outperform all other months, making this a plannable demand pattern
- **Central region underperforms on margin, not volume** — sales are competitive but profit is disproportionately low, suggesting aggressive discounting in that region

---

## ⚙️ Tech Stack

| Tool | Role |
| --- | --- |
| Python (Pandas, NumPy) | Data loading, cleaning, transformation, and aggregation |
| Matplotlib | Core charting — histograms, bar charts, line charts, scatter plots |
| Seaborn | Heatmaps and statistical visualizations |
| SciPy (stats) | Linear regression and p-value calculation for statistical validation |

---

## ▶️ How to Run

```bash
# 1. Clone the repo
git clone https://github.com/JasjotSingh17/superstore-eda.git
cd superstore-eda

# 2. Install dependencies
pip install pandas numpy matplotlib seaborn scipy jupyter

# 3. Download the dataset from Kaggle and place it in the project folder
# https://www.kaggle.com/datasets/vivek468/superstore-dataset-final
# File name: Sample - Superstore.csv

# 4. Launch the notebook
jupyter notebook superstore_eda.ipynb
```

> The dataset is not included in this repository as it is sourced from Kaggle. Download it from the link above and place it in the same folder as the notebook before running.

---

## 👤 Author

**Jasjot Singh**
University of Waterloo — BMath, Mathematical Studies (Minor: Computer Science)
[LinkedIn](https://linkedin.com/in/your-profile) | j367sing@uwaterloo.ca
