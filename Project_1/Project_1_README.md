# Project 1 — Retail Sales & Profit Analysis

## Why I Built This
Retail businesses often struggle to identify which regions and product categories actually drive profit — not just revenue. I wanted to dig into a real sales dataset and find out where the money actually comes from, and where it's being lost to discounts.

## Business Questions
- Which region generates the highest sales?
- Which product category is the most profitable?
- Which products generate the highest revenue?
- Which customer segment contributes the most profit?
- What is the monthly sales trend?

## Dataset
| Detail | Value |
|--------|-------|
| Source | Retail Sales — Orders, Customers, Products, Regions |
| Total Rows | 8,399 |
| Original Columns | 21 |
| Final Columns | 22 |
| Added Feature | `Year_Month` (derived from Order Date) |

## Data Cleaning
- Removed duplicate records
- Numeric columns converted and missing values filled (Product Base Margin filled with median)
- Categorical columns filled with 'Unknown' where missing
- Date columns formatted to datetime
- Column names standardized (spaces replaced with underscores)

## Key Findings

| Metric | Value |
|--------|-------|
| Total Sales | $14.92M |
| Total Profit | $1.52M |
| Average Discount | 4.97% |
| Top Region | West |
| Top Category | Technology |
| Most Profitable Segment | Corporate |

## Data Insights
- Technology generated the highest sales across all product categories
- West region recorded the highest sales among all regions
- Corporate customers generated the highest profit
- Furniture had high sales volume but relatively low profit margins
- Average discount is well controlled at 4.97%

## Business Insights
- Technology is the best-performing product category — scale investment here
- Corporate is the most profitable customer segment — prioritise retention
- Furniture sales are high but profitability is comparatively low — review pricing or cost structure
- West region dominates — analyse what makes it work and replicate in low-performing regions

## Recommendations
- Increase Technology product range and marketing spend
- Offer loyalty programmes to Corporate segment customers
- Review Furniture margins — either raise prices or reduce supplier costs
- Investigate high-discount orders — discounts above a threshold may be hurting profit

## Risks Identified
- High dependence on Technology category — single-category risk
- Low sales in some regions — growth opportunity being missed
- High discounts in certain orders could reduce profitability

## Tools Used
`Python` · `pandas` · `numpy` · `matplotlib`
