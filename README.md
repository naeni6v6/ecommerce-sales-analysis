# 🛒 E-Commerce Sales Data Analysis

## Overview
Data analysis project aimed at maximizing e-commerce revenue
through EDA, RFM-based customer segmentation, and marketing strategy proposals.

**Goal**: Develop strategies to increase total sales by 15% YoY

## Team
- Nayeon Kim, Yeonjae Oh, Doyoung Lee

## Dataset
- Name: ecommerce_sales_34500.csv
- Size: 34,500 transactions (2023–2025)
- Key Variables: price, discount, quantity, total_amount, profit_margin,
  customer_age, customer_gender, region, payment_method

## Analysis Structure

### 1. EDA (Exploratory Data Analysis)
- No missing values or duplicates → high data quality
- price & total_amount follow long-tail distribution
- Top 10% high-value customers account for majority of revenue

### 2. Visualization & Grouping
| Analysis | Key Finding |
|----------|-------------|
| Sales by Region | West & South regions show highest average purchase amount |
| Sales by Category | Electronics: low order count but highest revenue contribution |
| Sales by Gender | Nearly equal distribution (Male 47.6% / Female 48.6%) |
| Sales by Age Group | 20s customers show highest purchase amount and frequency |

### 3. RFM Analysis
Customer segmentation using Recency, Frequency, Monetary metrics
with optimized weights based on data distribution:

**Weight: R : F : M = 2 : 1 : 4**
(Monetary weighted highest due to long-tail distribution)

| Segment | Customers | Avg Recency | Avg Monetary | Revenue Contribution |
|---------|-----------|-------------|--------------|----------------------|
| VIP | 795 | 46 days | $2,292 | 31.07% |
| Excellent | 2,435 | 86 days | $1,004 | 41.67% |
| General | 1,988 | 158 days | $541 | 18.33% |
| Churned | 2,685 | 259 days | $195 | 8.94% |

### 4. Marketing Strategy
| Segment | Strategy |
|---------|----------|
| VIP | Loyalty program, personalized recommendations, dedicated service |
| Excellent | Upselling/cross-selling, VIP conversion campaign |
| General | Re-purchase coupons, bundle discounts, newsletter engagement |
| Churned | Win-back campaign, welcome-back coupons, push notifications |

## Key Insights
- Top 10% high-value customers drive majority of total revenue
- Electronics category shows highest revenue despite lower order count
- Monetary value is the strongest predictor of customer contribution
- Excellent segment (41.67% revenue) has highest VIP conversion potential

## Tech Stack
- Python, Pandas, Matplotlib, Seaborn
- RFM Analysis, EDA, Customer Segmentation
