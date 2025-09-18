# Customer Segmentation & RFM Analysis (SQL + Python)

## Project Overview
This project analyzes **customer transaction data** from an online retail dataset to perform **RFM (Recency, Frequency, Monetary) segmentation**.  
The goal is to identify high-value, medium-value, and low-value customers for better **marketing strategy and resource allocation**.

The analysis is done **primarily in SQL** (SQLite) with **Python** used for visualization and storytelling.

---

## Business Problem
The company currently treats all customers the same, regardless of their purchase behavior.  
However, not all customers are equally valuable:
- Some purchase frequently and spend a lot (high-value).
- Others only buy once or haven’t returned in a long time (low-value).  

The challenge is to **segment customers** based on behavior and identify opportunities for:
- Loyalty programs
- Targeted promotions
- Win-back campaigns for at-risk customers

---

## Tools & Skills Used
- **SQL (SQLite)** → data cleaning, RFM calculation, segmentation
- **Python (Pandas, Matplotlib, Seaborn)** → visualization & storytelling
- **Business Analytics** → marketing recommendations from data

---

## Project Steps
1. **Data Loading & Cleaning**
   - Removed canceled orders, negative quantities, and null customer IDs.
   - Created a cleaned SQL view (`retail_clean`).

2. **Exploratory Analysis (SQL)**
   - Revenue contribution by country
   - Total revenue and unique customers

3. **RFM Calculation (SQL)**
   - Recency = days since last purchase
   - Frequency = number of unique invoices
   - Monetary = total revenue per customer

4. **RFM Segmentation (SQL + Window Functions)**
   - Customers scored (1–4) for each dimension
   - Combined into an RFM segment and score

5. **Visualization (Python)**
   - Histograms of R, F, M
   - Heatmap of average spend by recency/frequency
   - Scatter plot of frequency vs monetary

6. **Business Insights**
   - High-value customers identified → retention programs
   - Medium-value customers → nurturing strategies
   - Low-value customers → win-back or deprioritize

---

## Key Insights
- A small group of **high RFM customers** generates a large share of revenue.
- Most customers purchase only once or twice, suggesting **low loyalty**.
- The **UK dominates revenue**, but there are strong opportunities in other top-5 countries.

---

## Recommendations
1. **High-Value Customers**
   - Reward with loyalty benefits and VIP access.
2. **Medium-Value Customers**
   - Encourage repeat purchases with promotions.
3. **Low-Value / At-Risk Customers**
   - Use re-engagement campaigns or reduce spend on them.
4. **Geographic Focus**
   - Expand campaigns outside the UK to grow global sales.

---

## Value for Employers
This project demonstrates:
- Proficiency in **SQL queries, window functions, and views**
- Ability to connect **SQL results to business insights**
- Skills in **data visualization and marketing analytics**
- Clear **end-to-end workflow** from raw data → insights → recommendations
