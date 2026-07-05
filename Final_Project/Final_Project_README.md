# Final Project — Store Sales Forecasting & Demand Prediction

## Why I Built This
This is my most complex project. I wanted to work with a real-world large-scale retail dataset — not a clean 1,000-row file, but millions of records across multiple tables. The goal was to understand how stores, products, seasons, and holidays together drive sales — and build insights that a retail operations team could actually act on.

## Business Goal
Build a dashboard to monitor sales performance, customer demand, seasonal trends, and future sales forecasts across a multi-store retail chain.

## Business Questions
- Which product families drive the most revenue?
- Which stores perform best — and why?
- How do holidays and seasons affect sales?
- Which cities generate the highest demand?
- How can inventory and promotions be planned around demand patterns?

## Dataset
| Detail | Value |
|--------|-------|
| Source | Store Sales Forecasting & Demand Prediction (Kaggle) |
| Source Files | train.csv, stores.csv, transactions.csv, holidays_events.csv |
| Final Merged Dataset | 3,054,348 rows × 25 columns |
| Stores | 54 |
| Product Families | 33 |
| Cities | 22 |
| States | 16 |

## Feature Engineering
Added 8 new time-based features from the date column:

| Feature | Description |
|---------|-------------|
| `Year` | Extracted year |
| `Month` | Month number |
| `Month_Name` | Month name |
| `Week` | Week number |
| `Day` | Day of month |
| `Day_Name` | Day name |
| `Quarter` | Q1–Q4 |
| `Weekend` | Weekend flag (1/0) |
| `Holiday_Flag` | Holiday flag from holidays dataset |

## Data Cleaning
- Duplicate records removed across all 4 datasets
- Missing numeric values filled with 0
- Missing categorical values filled with 'Unknown'
- All date columns formatted to datetime
- Datasets merged on store number and date

## Key Findings

| Metric | Value |
|--------|-------|
| Total Sales | ~$1.10 Billion |
| Total Transactions | 4.76 Billion+ |
| Top Product Family | Grocery I (32% of total revenue) |
| Top Store | Store 44 |
| Top City | Quito |
| Highest Sales Month | July |
| Highest Sales Quarter | Q2 |

## Data Insights
- Total sales reached approximately **$1.10 Billion** across the full dataset
- Total transactions exceeded **4.76 Billion**
- Grocery I alone contributed nearly **32%** of total revenue — the single biggest driver
- Store 44 recorded the highest sales among all 54 stores
- Quito generated the highest sales among all 22 cities
- July was the peak month; Q2 was the highest-performing quarter overall

## Business Insights
- Grocery I is the main revenue driver and must remain a business priority — any stockout here directly impacts overall performance
- Sales increase during specific months, showing clear seasonal demand patterns that can be planned for
- Quito and the top-performing stores contribute a disproportionate share of total sales
- Promotions support sales growth for high-demand product families — particularly effective for Grocery I

## Recommendations
- Increase inventory for Grocery I and other high-selling product families ahead of Q2 and July peaks
- Analyse Store 44's operations — understand what makes it the top performer and replicate across lower stores
- Build a promotion calendar aligned to seasonal peaks (Q2, July) to maximise conversion
- Invest in demand forecasting for the top 5 product families to reduce both stockout and overstock risk
- Expand operations or marketing presence in Quito and top cities to consolidate the sales advantage

## Risks Identified
- Heavy dependence on Grocery I for overall sales — single-category concentration risk
- Low-performing stores may drag down overall business growth if not addressed
- Seasonal demand fluctuations can cause inventory planning failures if not tracked proactively

## Tools Used
`Python` · `pandas` · `numpy` · `matplotlib`

## Project Complexity
This project involved working with **3 million+ rows** across **4 merged datasets** — the largest and most technically demanding project in this portfolio.
