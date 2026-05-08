# 🛍️ Customer Shopping Behavior Analysis

A data analysis project exploring shopping patterns, customer segments, and product preferences using transactional retail data.

---

## 📌 Project Overview

Analyzed 3,900 customer purchase records to uncover actionable business insights across demographics, product categories, and subscription behavior.

---

## 🗂️ Dataset

| Detail | Info |
|---|---|
| Records | 3,900 rows |
| Features | 18 columns |
| Missing Data | 37 values in Review Rating (imputed) |

**Key columns:** Age, Gender, Location, Item Purchased, Category, Purchase Amount, Season, Subscription Status, Discount Applied, Review Rating, Shipping Type, Payment Method

---

## 🛠️ Tools & Technologies

- **Python** (pandas) — data cleaning & feature engineering
- **PostgreSQL** — SQL-based business analysis
- **Power BI** — interactive dashboard

---

## 🔍 Process

### 1. Data Cleaning (Python)
- Imputed missing Review Ratings using median per product category
- Renamed columns to snake_case
- Dropped redundant `promo_code_used` column (identical to `discount_applied`)

### 2. Feature Engineering
- Created `age_group` column by binning customer ages
- Created `purchase_frequency_days` from purchase frequency data

### 3. SQL Analysis (PostgreSQL)
Answered 10 key business questions:

| # | Question |
|---|---|
| 1 | Revenue by Gender |
| 2 | High-Spending Discount Users |
| 3 | Top 5 Products by Rating |
| 4 | Standard vs. Express Shipping Comparison |
| 5 | Subscribers vs. Non-Subscribers |
| 6 | Most Discount-Dependent Products |
| 7 | Customer Segmentation (New / Returning / Loyal) |
| 8 | Top 3 Products per Category |
| 9 | Repeat Buyers & Subscription Likelihood |
| 10 | Revenue by Age Group |

### 4. Dashboard (Power BI)
Built an interactive dashboard with filters for gender, subscription status, category, and shipping type.

---

## 📊 Key Findings

- **Male customers** generated significantly higher revenue ($157,890) vs. female ($75,191)
- **839 customers** used discounts but still spent above average — high-value discount users
- **Top-rated products:** Gloves (3.86), Sandals (3.84), Boots (3.82)
- **Express shipping** users spend slightly more on average ($60.48 vs $58.46 for Standard)
- **Subscribers vs. Non-subscribers** have nearly identical average spend (~$59), suggesting subscriptions aren't tied to higher spending
- **80% of customers** (3,116) fall into the Loyal segment
- **Young Adults** are the top revenue-generating age group ($62,143)

---

## 💡 Business Recommendations

1. **Boost Subscriptions** — Promote exclusive perks; subscribers currently behave like non-subscribers
2. **Loyalty Programs** — Reward repeat buyers to accelerate their move into the Loyal segment
3. **Revisit Discount Policy** — High discount rates on Hats (50%) and Sneakers (49.66%) may be eroding margins
4. **Targeted Campaigns** — Focus on Young Adults and Express Shipping users, who show higher spending
5. **Highlight Top Products** — Feature Gloves, Sandals, and Boots prominently in marketing

---

## 📁 Project Structure

```
├── data/               # Raw and cleaned datasets
├── notebooks/          # Python EDA scripts
├── sql/                # SQL queries
├── dashboard/          # Power BI file (.pbix)
└── README.md



<img width="1295" height="730" alt="Dashboard SS" src="https://github.com/user-attachments/assets/847adf20-4793-4abc-ab62-f1b93245cb73" />



```
