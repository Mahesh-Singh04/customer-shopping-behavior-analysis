# 🛍️ Customer Shopping Behavior Analysis

An end-to-end data analytics project analyzing customer shopping patterns across 3,900 transactions — covering Python data cleaning, SQL business analysis, and an interactive Power BI dashboard.

---

## 📌 Project Overview

This project uncovers insights into customer spending patterns, product preferences, customer segmentation, and subscription behavior using real transactional retail data. The goal is to help businesses make smarter, data-driven decisions.

### 🔄 Project Workflow

<img width="4872" height="2656" alt="Project Overview" src="https://github.com/user-attachments/assets/7bfef409-5dd3-4721-8c26-028efd3a8a21" />


| Step | Phase | Description |
|---|---|---|
| 01 | Business Problem Statement | Defined the business questions to answer |
| 02 | Data Modelling & EDA in Python | Imported data, cleaned and explored using Python |
| 03 | Data Analysis in SQL | Loaded data into MySQL and ran business queries |
| 04 | Interactive Dashboard in Power BI | Connected MySQL to Power BI and built dashboard |
| 05 | Project Report | Summarized all findings into a detailed report |
| 06 | Presentation using Gamma AI | Presented insights to stakeholders |
| 07 | GitHub Repository | Uploaded all project files to GitHub |

---

## 🛠️ Tools & Technologies

| Tool | Purpose |
|---|---|
| Python (Pandas, NumPy) | Data Cleaning & Feature Engineering |
| MySQL | Database Storage & SQL Analysis |
| Power BI | Interactive Dashboard & Visualizations |

---

## 📁 Project Structure

```
customer-shopping-behavior-analysis/
│
├── README.md
├── LICENSE
├── customer_shopping_behavior_data.csv
├── customer_shopping_behavior_analysis_jupyterNotebook.ipynb
├── customer_shopping_behavior_sql_quaries.sql
├── Customer_Shopping_Behavior_dashboard.pbix
├── Customer_Shopping_Behavior_Analysis_Report.pdf
├── Business Problem Document.pdf
└── Customer-Shopping-Behavior-Analysis.pptx
```

---

## 📊 Dataset Summary

- **Rows:** 3,900 transactions
- **Columns:** 18 features
- **Key Features:**
  - Customer demographics — Age, Gender, Location, Subscription Status
  - Purchase details — Item Purchased, Category, Purchase Amount, Season, Size, Color
  - Shopping behavior — Discount Applied, Previous Purchases, Frequency, Review Rating, Shipping Type
- **Missing Data:** 37 null values in Review Rating (handled via category-wise median imputation)

---

## 🔧 Phase 1 — Data Cleaning (Python)

- Loaded dataset using **Pandas** and performed initial exploration with `df.info()` and `.describe()`
- Imputed missing **Review Rating** values using **group-wise median** per product category
- Renamed all columns to **snake_case** for consistency
- **Feature Engineering:**
  - Created `age_group` column by binning customer ages
  - Created `purchase_frequency_days` column from purchase frequency data
- Dropped redundant `promo_code_used` column (duplicate of `discount_applied`)
- Loaded the cleaned DataFrame into **MySQL** for SQL analysis

---

## 🗃️ Phase 2 — SQL Analysis (MySQL)

Answered 10 key business questions using structured SQL queries:

| # | Analysis | Key Finding |
|---|---|---|
| 1 | Revenue by Gender | Male: $157,890 \| Female: $75,191 |
| 2 | High-Spending Discount Users | 839 customers used discounts but spent above average |
| 3 | Top 5 Products by Rating | Gloves (3.86), Sandals (3.84), Boots (3.82), Hat (3.80), Skirt (3.78) |
| 4 | Shipping Type Comparison | Express ($60.48) slightly higher than Standard ($58.46) |
| 5 | Subscribers vs Non-Subscribers | Similar avg spend (~$59); non-subscribers drive 73% of revenue |
| 6 | Discount-Dependent Products | Hat (50%), Sneakers (49.66%), Coat (49.07%) top discount reliance |
| 7 | Customer Segmentation | Loyal: 3,116 \| Returning: 701 \| New: 83 |
| 8 | Top 3 Products per Category | Jewelry, Blouse, Sandals, Jacket lead their categories |
| 9 | Repeat Buyers & Subscriptions | 2,518 repeat buyers are non-subscribers — big opportunity |
| 10 | Revenue by Age Group | Young Adults lead at $62,143 followed by Middle-aged at $59,197 |

---

## 📈 Phase 3 — Power BI Dashboard

Built an interactive **Customer Behavior Dashboard** featuring:

- **KPI Cards** — Total Customers (3.9K), Avg Purchase Amount ($59.76), Avg Review Rating (3.75)
- **Donut Chart** — Subscription Status split (Yes 27% / No 73%)
- **Bar Charts** — Revenue by Category, Sales by Category
- **Horizontal Bar Charts** — Revenue by Age Group, Sales by Age Group
- **Slicers/Filters** — Subscription Status, Gender, Category, Shipping Type

><img width="572" height="327" alt="Customer_behavior_analysis_dashboard" src="https://github.com/user-attachments/assets/fc6154e8-c930-4075-b1b6-085b5c0feb5f" />


---

## 💡 Key Business Insights

- 📦 **Clothing** is the top revenue-generating category
- 👨 **Male customers** generate significantly more revenue than female customers
- 🎯 **73% of customers are non-subscribers** — a major growth opportunity for subscription campaigns
- 🔄 **80% of customers are Loyal** (3,116 out of 3,900) — strong retention base
- 💸 **839 discount users** still spend above average — discounts don't always reduce margins
- 🧑 **Young Adults** are the highest revenue age group ($62,143)

---

## ✅ Business Recommendations

1. **Boost Subscriptions** — Promote exclusive subscriber benefits to convert the 73% non-subscribers
2. **Customer Loyalty Programs** — Reward repeat buyers to grow the Loyal segment further
3. **Review Discount Policy** — High-discount products like Hat and Sneakers need margin evaluation
4. **Product Positioning** — Highlight top-rated products (Gloves, Sandals) in marketing campaigns
5. **Targeted Marketing** — Focus on Young Adults and Express-shipping users for premium campaigns

---

## 🚀 How to Run This Project

1. Clone the repository
```bash
git clone https://github.com/Mahesh-Singh04/customer-shopping-behavior-analysis.git
cd customer-shopping-behavior-analysis
```

2. Run the data cleaning notebook
```bash
jupyter notebook customer_shopping_behavior_analysis_jupyterNotebook.ipynb
```

3. Load `customer_shopping_behavior_data.csv` into MySQL and run `customer_shopping_behavior_sql_quaries.sql`

4. Open `Customer_Shopping_Behavior_dashboard.pbix` in Power BI Desktop

---

## 📬 Connect with Me

- 💼 **LinkedIn:** [linkedin.com/in/mahesh-singh04](https://www.linkedin.com/in/mahesh-singh04)
- 🐙 **GitHub:** [github.com/Mahesh-Singh04](https://github.com/Mahesh-Singh04)

---

## 📄 License

This project is licensed under the **MIT License** — feel free to use and learn from it.<img width="572" height="327" alt="Customer_behavior_analysis_dashboard" src="https://github.com/user-attachments/assets/4d01b2db-5274-4e4c-a8ca-1b67b3ed8bca" />
<img width="572" height="327" alt="Customer_behavior_analysis_dashboard" src="https://github.com/user-attachments/assets/dd4f5b09-381d-43bd-b1f3-ee83268cd74e" />
