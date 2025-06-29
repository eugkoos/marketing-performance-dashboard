# 📊 Marketing Campaign Performance Dashboard

**Author:** Eugene Kostiuchenko  
**Role:** Junior BI Analyst & Data Analyst  
**Tools:** Tableau (Calculated Fields, Parameters, Filters, Dashboard Design)  

## Project Summary

This project analyzes the performance of 11 marketing campaigns across 4 marketing channels over a 28-day period.  
The goal is to calculate advanced marketing KPIs, identify key trends, and present actionable insights in an interactive Tableau dashboard.

The dataset includes daily campaign metrics such as impressions, clicks, leads, orders, revenue, and marketing spend.  
All calculations were implemented using Tableau’s calculated fields.

## Dataset Overview

Each row represents a **daily snapshot** of a marketing campaign.

| Column         | Description                            |
|----------------|----------------------------------------|
| `date`         | Campaign date                          |
| `campaign_name`| Name of the marketing campaign          |
| `category`     | Marketing channel (search, social, etc.)|
| `impressions`  | Daily ad impressions                   |
| `clicks`       | Daily ad clicks                        |
| `leads`        | Daily leads (contact submissions)      |
| `orders`       | Daily completed purchases              |
| `revenue`      | Daily revenue                          |
| `spend`        | Daily marketing spend                  |
| `campaign_id`  | Unique campaign identifier             |

Dataset Source: https://www.kaggle.com/datasets/sinderpreet/analyze-the-marketing-spending  
*Note: Monetary values are displayed in USD ($) for readability only. The original dataset was in INR and not converted.*

## KPIs Calculated

| Metric            | Formula                             | Description                                      |
|-------------------|--------------------------------------|--------------------------------------------------|
| **ROMI**          | `(revenue - spend) / spend`          | Return on Marketing Investment                   |
| **Profit**        | `revenue - spend`                    | Gross profit after deducting marketing spend     |
| **CTR**           | `clicks / impressions`               | Click-through rate                               |
| **Click-to-Lead** | `leads / clicks`                     | Conversion from clicks to leads                  |
| **Click-to-Sale** | `orders / clicks`                    | Conversion from clicks to purchases              |
| **CPC**           | `spend / clicks`                     | Cost per click                                   |
| **CPL**           | `spend / leads`                      | Cost per lead                                    |
| **CAC**           | `spend / orders`                     | Customer acquisition cost                        |
| **AOV**           | `revenue / orders`                   | Average order value                              |

## Dashboard Highlights

📍 **Live dashboard:** [View on Tableau Public](https://public.tableau.com/app/profile/eugkoos/viz/MarketingPerformance_17511974263820/Dashboard)

Key Features:
- **KPI Tiles:** Display key metrics such as ROMI, Spend, Profit, Orders, CAC — with clear formatting and color indicators (e.g., red for negative profit).
- **Comparison Table:** Metrics are organized to reflect financial performance, efficiency, and traffic quality — helping to compare campaigns more easily.
- **Switchable View:** Users can toggle between Channel-level and Campaign-level views using a parameter control.
- **Time Series Charts:** Trends for ROMI, Spend, Orders, and CTR shown over time.
- **Interactive Controls:** Filters for Date, Channel, and Campaign; a reset button clears selections for easy navigation.
- **User-Friendly UX:** Metric tooltips offer quick definitions; unnecessary controls are hidden for a clean, focused layout.

## Key Insights

- **Influencer channel:** campaigns: highest ROMI (+154%), high AOV, lowest CAC  
- **Social channel:** campaigns: negative ROMI (–14%), highest cost metrics  
- **Media channel:** strong conversion rates, moderate profit  
- **Search channel:** balanced spend and return, steady performance  

## Repository Structure

| Path              | Description                          |
|-------------------|--------------------------------------|
| `data/`           | Raw dataset used for analysis        |
| `assets/`         | Dashboard screenshots                |
| `README.md`       | Full project documentation           |

## Links

- [Tableau Dashboard](https://public.tableau.com/app/profile/eugkoos/viz/MarketingPerformance_17511974263820/Dashboard)  
- [LinkedIn](https://www.linkedin.com/in/eugenekos/)  