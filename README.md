# Market Demand Forecasting and Pricing Intelligence Using Proxy Data
### MSc Dissertation · Published: Edward Elgar Publishing (2025)
### Python · XGBoost · Random Forest · Feature Engineering · 
### Geospatial Analysis · Time-Series Analysis

---

## Overview

This project solves a real forecasting problem in data-scarce 
environments: how do you forecast demand when direct demand 
data doesn't exist?

Using long-term Airbnb listing data for London (2008–2023), I 
engineered proxy demand signals from available listing 
characteristics - reviews, availability, pricing trends, 
minimum-night rules - and built predictive models to estimate 
demand patterns and pricing dynamics across London's 
short-term rental market.

This work was completed as my MSc dissertation at Alliance 
Manchester Business School and was subsequently selected for 
academic publication with Edward Elgar Publishing (2025).

**Tools:** Python · XGBoost · Random Forest · Decision Tree · 
Feature Engineering · Geospatial Analysis · RMSE · R²

---

## Publication

> **Chapter 4** in *"Forecasting, Planning and Strategy 
> in a Turbulent Era"*
> Edward Elgar Publishing Ltd. · May 2025
> [View publication](https://www.e-elgar.com/shop/gbp/forecasting-planning-and-strategy-in-a-turbulent-era-9781035317233.html)

Due to publishing agreements, raw datasets and full model 
code cannot be publicly shared. This repository focuses on 
methodology, analytical approach, and business insights.

---

## Business Problem

Short-term rental platforms, hospitality businesses, and 
marketplace operators face a persistent data limitation: 
direct booking demand data is either unavailable, restricted, 
or unreliable.

Yet strategic decisions - pricing, supply planning, 
neighbourhood investment, policy response - all depend on 
understanding demand patterns.

Key questions this project addresses:

- How can demand be estimated reliably without direct 
  booking data?
- Which listing features and geographic factors drive 
  pricing and demand?
- How do demand patterns differ across London's 
  Inner vs. Outer markets?
- How can proxy-based demand signals support dynamic 
  pricing and supply planning decisions?

---

## Analytical Approach

**Demand Proxy Engineering**
Rather than using bookings (unavailable), I engineered 
proxy demand signals from observable listing data:
- Review count and recency as booking activity proxies
- Availability (90-day rule constraint) as demand signal
- Price dynamics as revealed preference indicator
- Minimum-night rules as host-side demand filtering

**Feature Engineering & Market Segmentation**
- Listing-level features: beds, bedrooms, bathrooms, 
  listing type, minimum nights, availability
- Geographic segmentation: Inner London vs. Outer London, 
  neighbourhood-level aggregation
- Listing type classification: entire home, private room, 
  shared room

**Predictive Modelling**

| Model | Performance |
|---|---|
| Decision Tree | Baseline benchmark |
| Random Forest | Improved accuracy over baseline |
| **XGBoost** | **Best-performing model ✓** |

Models evaluated using RMSE and R² to identify the most 
robust forecasting approach for proxy-based demand estimation.

---

## Key Findings

**Inner London commands ~25% price premium over Outer London**
Geographic segmentation revealed significant and consistent 
price differentials between Inner and Outer London - 
supporting differentiated pricing strategy and 
neighbourhood-level investment decisions.

**Listing type is the strongest demand and pricing driver**
Entire homes and private rooms showed significantly 
different demand behaviour, pricing elasticity, and 
availability patterns - meaning listing type should 
be the primary segmentation variable for any pricing 
or supply planning model.

**Availability and minimum-night rules materially 
distort demand signals**
The 90-day rule creates systematic availability 
constraints that affect how demand proxies behave - 
a critical methodological insight for anyone building 
demand models on Airbnb data.

**XGBoost outperforms simpler models for proxy-based 
demand forecasting**
The non-linear relationships between listing features 
and demand proxies make tree-based ensemble methods 
significantly more effective than linear or 
single-tree approaches.

---

## Strategic Recommendations

For marketplace and hospitality platforms operating 
in data-scarce environments:

- Deploy dynamic pricing models segmented by 
  neighbourhood and listing type rather than 
  platform-wide pricing
- Use proxy demand signals to simulate supply-demand 
  balance where direct booking data is restricted 
  or unavailable
- Target premium inventory investment in high-demand 
  central locations based on proxy-validated demand signals
- Incentivise supply in underutilised outer regions 
  to smooth demand concentration and reduce 
  peak-period pressure
- Use data-backed analysis to engage policymakers 
  on regulatory impact (e.g., 90-day rule effects 
  on supply and pricing)

---

## Tools & Technologies

| Tool | Usage |
|---|---|
| Python | Data processing, feature engineering, modelling |
| XGBoost | Best-performing demand proxy model |
| Random Forest | Ensemble benchmark model |
| Decision Tree | Baseline model |
| Geospatial Analysis | Inner/Outer London segmentation |
| Time-Series Analysis | Temporal demand pattern identification |
| RMSE + R² | Model evaluation and selection |

---

## Why This Project Is Distinctive

Most analytics projects work with clean, direct data. 
This project addresses the harder and more common 
real-world problem: building reliable forecasts when 
the data you actually need doesn't exist.

The proxy variable engineering methodology developed 
here is directly applicable to any marketplace, 
platform, or business where demand must be inferred 
from observable signals rather than measured directly.

This approach was considered sufficiently rigorous 
and original to be selected for peer-reviewed 
academic publication - one of the few analyst 
portfolios backed by published research.

---

*Part of the E-Commerce & Supply Chain Analytics Portfolio*
*[View full portfolio](https://aarushijainportfolio.netlify.app/)*
