# Market-Demand-and-Pricing-Forecasting (Airbnb)

# Overview

This project demonstrates how market demand and pricing insights can be forecasted even when direct demand data is unavailable, a common challenge in real-world marketplaces.

Using Python and machine learning, I analysed long-term Airbnb listing data for London to:

- Identify key demand and pricing drivers

- Understand spatial and seasonal demand patterns

- Build robust predictive models for price and demand proxies

This work was completed as part of my MSc dissertation and was later selected for academic publication due to its methodological and business relevance.

# Business Problem

Short-term rental platforms and hospitality businesses often face a critical limitation:

- Demand data is incomplete, noisy, or unavailable.

Yet strategic decisions still depend on understanding:

- Where demand concentrates geographically

- Which listing features truly drive pricing and demand

- How demand differs across market segments

- How to simulate demand for pricing, supply planning, and policy decisions

This project addresses:

- How to forecast demand indirectly using proxy signals

- How to turn listing and availability data into decision-ready insights

# Solution Approach

I designed a demand and pricing forecasting framework using Airbnb listing data spanning 2008–2023.

**🔹 Demand Proxy Design**

- Used price, availability, and listing characteristics as demand proxies

- Incorporated constraints such as the 90-day rule affecting bookings

**🔹 Feature Engineering & Market Segmentation**

- Minimum nights, availability (90 days), beds, bedrooms, bathrooms

- Listing type (entire home, private room, shared room)

- Geographic segmentation: Inner vs. Outer London

- Neighbourhood-level aggregation for spatial insights

**🔹 Predictive Modeling**

- Built and compared multiple machine learning models:

- Decision Tree

- Random Forest

- XGBoost (best-performing model)

Models were evaluated using RMSE and R² to identify the most robust forecasting approach.

# Key Busines Insights and Impact

- Inner London listings commanded ~25% higher prices than Outer London
 → Supports premium pricing and differentiated marketing strategies

- Listing type was the strongest driver of demand and pricing
 → Entire homes and private rooms showed significantly different demand behavior

- Availability and minimum-night rules materially affected demand signals
 → Critical inputs for supply simulation and policy evaluation

- XGBoost delivered the most reliable forecasts, outperforming simpler models
 → Suitable for scaling dynamic pricing and demand simulation tools

# Strategic Recommendations

Based on the analysis, the following actions were identified for marketplace and hospitality platforms:

- Deploy dynamic pricing models tailored by neighbourhood and listing type

- Use demand proxies to simulate supply–demand balance where bookings data is restricted

- Target premium segments in high-value central locations

- Incentivize demand in underutilized outer regions to smooth supply pressure

- Engage with policymakers using data-backed insights (e.g., 90-day rule impact)

# Tools and Technologies

- Python

- Machine Learning: Decision Trees, Random Forest, XGBoost

- EDA & Feature Engineering

- Geospatial & Time-Series Analysis

- Forecasting & Model Evaluation (RMSE, R²)

# Why this Matters for Your Business

This project shows how to:

- Forecast demand when direct data is missing

- Support pricing, supply planning, and policy decisions

- Translate raw marketplace data into actionable growth insights

The same framework can be applied to:

- Short-term rental platforms

- Hospitality chains

- Marketplaces with incomplete demand signals

- City-level tourism and accommodation planning

# 📌 Publication Note

This work was selected for publication as Chapter 4 in
“[Planning, Forecasting and Strategy in a Turbulent Era” (Edward Elgar Publishing)](https://www.e-elgar.com/shop/gbp/forecasting-planning-and-strategy-in-a-turbulent-era-9781035317233.html?srsltid=AfmBOorYoYOmUQw3jcC1SZIoizarkhGIr29IqE7vXxdEQ8xUTVI7TFwP).

Due to publishing agreements, raw datasets and full code cannot be publicly shared.
This case study focuses on methodology, insights, and business impact.

# 💬 How I Can Help You

If your business needs to:

- Forecast demand without clean booking data

- Build pricing or supply simulation models

- Understand spatial and seasonal demand patterns

- Support strategy with data-backed forecasting

I can adapt this approach to your marketplace or hospitality data and deliver:

- Forecasting models

- Demand simulations

- Strategic insights for pricing and growth

