# Project 2 — E-Commerce Sales Analysis

## Why I Built This
E-commerce is one of India's fastest-growing sectors but most businesses don't know which states, categories, or payment methods are actually driving their numbers. I wanted to analyse a real Indian e-commerce dataset and find actionable patterns — especially around payment behaviour, which I suspected would be surprising.

## Business Questions
- Which state generates the highest sales?
- Which product category is most profitable?
- Which products generate the highest revenue?
- Which payment method is used the most?
- What is the monthly sales trend?

## Dataset
| Detail | Value |
|--------|-------|
| Source | E-Commerce Sales Dataset |
| Total Rows | 15,000 |
| Original Columns | 12 |
| Final Columns | 13 |
| Added Feature | `Year_Month` (derived from Order Date) |

## Data Cleaning
- Removed duplicate records
- Numeric columns (Quantity, Sales Amount, Discount, Profit) converted and nulls filled with 0
- Categorical columns (Product Category, State, City, Payment Mode) filled with 'Unknown'
- Order Date formatted to datetime
- Column names standardized

## Key Findings

| Metric | Value |
|--------|-------|
| Total Sales | $49.38M |
| Total Profit | $7.38M |
| Total Quantity Sold | 45,191 |
| Top State | Rajasthan |
| Top Category | Electronics |
| Top Payment Method | Cash on Delivery (COD) |

## Data Insights
- Rajasthan generated the highest sales among all states
- Electronics generated the highest profit across all categories
- Cash on Delivery was the most used payment method — despite being the riskiest for businesses
- Monthly sales remained relatively stable throughout the period
- Top-selling products contribute significantly to total revenue

## Business Insights
- Rajasthan is the best-performing state — worth deeper analysis to understand why
- Electronics dominates profit — this category needs priority stock and marketing
- COD dominance is a red flag — COD increases return rates and cash flow delays
- Stable monthly trend suggests consistent demand but no seasonal spike strategy in place

## Recommendations
- Push prepaid payment incentives (cashback, discounts) to shift customers away from COD
- Increase Electronics inventory ahead of peak months
- Launch targeted campaigns in low-performing states to reduce geographic concentration
- Introduce seasonal promotions to create demand spikes and improve monthly trend

## Risks Identified
- Heavy dependence on Electronics category — vulnerability if demand drops
- Sales concentrated in fewer states — geographic risk
- High COD reliance increases operational cost and return rates

## Tools Used
`Python` · `pandas` · `numpy` · `matplotlib`
