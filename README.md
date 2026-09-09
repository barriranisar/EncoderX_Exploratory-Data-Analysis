
---


# 📊 Exploratory Data Analysis (EDA) - Sample Superstore Dataset

> **EncoderX Remote Internship (Batch 02) — Track: Data Science**  
> **Task 01:** Exploratory Data Analysis & Business Intelligence  

---

## 📌 Project Overview
This project performs an in-depth **Exploratory Data Analysis (EDA)** on retail transaction data from a US-based Superstore. The goal is to uncover business trends, evaluate profit margins across product categories and sub-categories, analyze the financial impact of promotional discounts, and deliver data-backed recommendations to optimize profitability.

---

## 📁 Repository Structure

```text
├── data/
│   ├── SampleSuperstoreDataset.csv          # Raw Superstore Dataset (9,994 records)
│   └── Cleaned_SampleSuperstoreDataset.csv  # Cleaned Dataset (9,977 records)
├── notebooks/
│   └── EDA_Superstore.ipynb                 # Complete Jupyter Notebook with code & outputs
├── visualizations/
│   ├── 01_sales_profit_distribution.png     # Sales & Profit distribution histograms
│   ├── 02_subcategory_sales_profit.png      # Sales vs. Profit across Sub-Categories
│   ├── 03_scatter_sales_profit_discount.png # Sales vs. Profit scatter plot by discount
│   ├── 04_correlation_heatmap.png           # Feature correlation matrix heatmap
│   └── 05_discount_vs_profit_trend.png      # Discount rate vs. Average profit trend
├── report/
│   └── Superstore_EDA_Report.pdf            # Professional Executive Summary Report
└── README.md                                # Project documentation & findings

```

---

## ⚙️ Data Preprocessing & Cleaning Summary

* **Raw Dataset:** 9,994 entries, 13 features.
* **Cleaning Steps Taken:**
1. **Duplicate Records:** Identified and dropped `17` duplicate rows.
2. **Missing Value Audit:** Confirmed complete data integrity (0 null values across all columns).
3. **Feature Selection:** Pruned redundant single-value column `Country` ("United States") and non-analytical identifier `Postal Code`.
4. **Processed Dataset Export:** Saved clean data as `Cleaned_SampleSuperstoreDataset.csv` (`9,977` rows × `11` columns).



---

## 📈 Key Visualizations & Diagnostic Findings

| # | Visualization | Key Business Insight |
| --- | --- | --- |
| **1** | **Distribution Analysis (Histogram)** | Both `Sales` and `Profit` exhibit strong positive skewness. High-volume, low-ticket orders dominate transactions, with extreme outliers driving substantial revenue peaks. |
| **2** | **Sub-Category Breakdown (Bar Chart)** | **Phones**, **Chairs**, and **Storage** lead in sales volume. **Copiers** yield the highest profit margins, while **Tables** and **Bookcases** incur consistent net losses despite solid sales. |
| **3** | **Sales vs. Profit by Discount (Scatter Plot)** | Higher discount tiers (represented by darker hues) correlate directly with severe downward profit trajectories. |
| **4** | **Correlation Matrix (Heatmap)** | Demonstrates an inverse correlation between **Discount** and **Profit** ($r = -0.22$), proving that aggressive price slashing erodes overall bottom-line returns. |
| **5** | **Discount Threshold Curve (Line Chart)** | Pinpoints an inflexion point at **20% discount**: beyond 20%, average order profitability drops steadily into negative numbers. |

---

## 💡 Strategic Business Recommendations

1. **Implement a Discount Ceiling:** Cap promotional discounts at **15%–20%**. Any special discount exceeding 20% should require managerial approval to prevent negative-margin transactions.
2. **Restructure Loss-Making Categories:** Renegotiate supplier and fulfillment costs for **Tables** and **Bookcases**, or bundle them with high-margin items like **Copiers** and **Phones**.
3. **Focus on High-Yield Regions:** Prioritize marketing spend and inventory allocation toward the **West** and **East** regions, which generate the strongest profit margins.

---

## 🛠️ Tools & Technologies Used

* **Programming Language:** Python
* **Data Manipulation:** Pandas, NumPy
* **Visualization Libraries:** Matplotlib, Seaborn
* **Environment:** Jupyter Notebook / VS Code

---

## 🔗 Submission Links

* **GitHub Repository:** 
* **LinkedIn Post:** 
* **Demo Video Walkthrough:** 

---



