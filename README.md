# Consumer Shopping Behaviour Analysis

An end-to-end data analysis project on 3,900 real shopping transactions using Python, MySQL, and Power BI.

## Project Overview
This project analyses 3,900 purchases across different product categories to uncover insights about customer spending, discount behaviour, subscription patterns, and product performance.

**Tools Used:** Python (Pandas) · MySQL · Power BI

## Repository Structure
```
├── data_cleaning.ipynb        # Data cleaning & feature engineering
├── analysis_queries.sql       # 10 business queries in MySQL
└── dashboard.pbix             # Power BI dashboard
```

## Key Findings

| # | Finding |
|---|---------|
| 1 | Subscribers generate more revenue and spend more per purchase than non-subscribers |
| 2 | 27% of customers are subscribers — but they drive a disproportionate share of revenue |
| 3 | Discount-dependent products rely heavily on promotions to drive sales |
| 4 | Express shipping customers tend to spend more than Standard shipping customers |
| 5 | Middle-aged customers contribute the most to total revenue by age group |
| 6 | Average spend per purchase is $59.76 with an average review rating of 3.75 |

## What I Did

### Data Cleaning (Python)
- Loaded dataset with Pandas and explored structure using `.info()` and `.describe()`
- Fixed 37 missing Review Rating values using median per product category
- Renamed all columns to `snake_case` for consistency
- Engineered two new features: `age_group` and `purchase_frequency_days`
- Dropped `promo_code_used` as it was redundant with `discount_applied`
- Exported cleaned data into MySQL for analysis

### Business Queries (MySQL)
10 business queries were executed on the cleaned dataset:

| Query | Key Finding |
|-------|-------------|
| Revenue by Gender | Compared total spending between male and female customers |
| High-Spending Discount Users | Identified customers who used discounts but still spent above average |
| Top 5 Products by Rating | Found highest rated products across all categories |
| Shipping Type Comparison | Express vs Standard — who spends more? |
| Subscribers vs Non-Subscribers | Compared revenue and average spend |
| Discount-Dependent Products | Top 5 products most reliant on discounts |
| Customer Segmentation | Classified customers as New, Returning, or Loyal |
| Top 3 Products per Category | Best sellers within each product category |
| Repeat Buyers & Subscriptions | Do frequent buyers subscribe more? |
| Revenue by Age Group | Which age group contributes the most? |

### Dashboard (Power BI)
The Power BI dashboard includes interactive filters for gender, subscription status, category, and shipping type. It visualises:
- Revenue and sales by category and age group
- Subscription status breakdown (27% vs 73%)
- Review ratings by product category
- Discount usage patterns

## Actionables

**1. Target Non-Subscribers with Offers**
73% of customers are not subscribed. A targeted campaign offering a first-month discount could significantly boost subscription revenue.

**2. Reduce Discount Dependency**
Some products only sell well with discounts. Improving their visibility through better placement or bundling could reduce reliance on promotions.

---
Made by **Shristee** · [GitHub](https://github.com/shristee04)
