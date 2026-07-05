# Project 3 — Supply Chain & Inventory Analysis

## Why I Built This
Inventory mismanagement is one of the biggest silent cost drivers in any business — overstock wastes money, understock loses sales. I picked this dataset because I wanted to understand how data can be used to optimise inventory levels and evaluate supplier performance before problems hit the business.

## Business Questions
- Which products are frequently out of stock?
- Which suppliers have the highest delivery delays?
- Which products generate the highest profit?
- How can inventory be optimised?
- What is the impact of delivery delays on sales?

## Dataset
| Detail | Value |
|--------|-------|
| Source | Supply Chain & Inventory Dataset |
| Total Rows | 15,000 |
| Original Columns | 13 |
| Final Columns | 15 |
| Added Features | `Revenue`, `Profit`, `Delivery_Days` |

## Data Cleaning
- No duplicate records found
- Numeric columns validated and nulls filled with 0
- Categorical columns filled with 'Unknown' where missing
- Negative stock values identified and replaced with 0
- Date columns (Order Date, Delivery Date) formatted to datetime
- Column names standardized

## Key Findings

| Metric | Value |
|--------|-------|
| Total Revenue | $3.08 Billion |
| Total Profit | $612.92M |
| Total Units Sold | 2.22 Million |
| Average Shipping Time | 5.50 days |
| Top Supplier by Volume | Supplier E (452.8K units) |
| Highest Profit Product | Camera |
| Highest Inventory Location | Bangalore Warehouse |

## Data Insights
- Most products are currently **overstocked** — storage costs are higher than necessary
- Camera generated the highest total profit among all product categories
- Supplier E delivered the highest sales volume across all suppliers
- Average delivery time was consistent across all suppliers at ~5.5 days
- Bangalore warehouse stored the highest inventory among all locations

## Business Insights
- Overstock is the bigger problem than understock — working capital is being tied up unnecessarily
- Camera category is the profit engine — prioritise availability and avoid stockouts here
- Supplier E is the most reliable by volume — worth negotiating better rates given the relationship
- Uniform delivery time across suppliers suggests logistics, not suppliers, may be the bottleneck

## Recommendations
- Reduce excess inventory in overstocked categories to free up working capital and reduce storage costs
- Set camera stock as a priority — never allow Camera to go out of stock
- Conduct a reorder point review using current 90-day demand data
- Investigate delivery bottlenecks — if all suppliers deliver in ~5.5 days, the issue may be internal processing

## Risks Identified
- High overstock levels increasing storage and holding costs
- Some products require immediate restocking — risk of lost sales
- Delivery delays, even marginal ones, may impact customer satisfaction over time

## Tools Used
`Python` · `pandas` · `numpy` · `matplotlib`
