# Applied Time Series Analysis – Final Project

This repository showcases a **complete, end-to-end time series forecasting project** completed as part of a graduate-level **Applied Time Series Analysis** course in the M.S. in Applied Data Science program at the University of San Diego.

The project demonstrates how classical time series methods can be applied to real operational data to support forecasting, planning, and decision-making under volatility.

---

## Project Objective

The Transportation Security Administration (TSA) screens millions of passengers daily across U.S. airports. Passenger volumes follow predictable seasonal patterns but are also disrupted by external shocks such as pandemics, government shutdowns, and extreme weather events.

The goal of this project was to:

- Understand historical TSA passenger demand patterns  
- Identify trends, seasonality, and structural breaks in the data  
- Apply appropriate time series forecasting techniques  
- Evaluate model performance under both stable and volatile conditions  
- Translate forecasts into insights relevant for workforce planning  

---

## What This Repository Contains

- A **fully documented analysis notebook** containing:
  - Data ingestion and preprocessing  
  - Exploratory time series analysis and visualization  
  - Trend and seasonality decomposition  
  - Time series model development (ETS and ARIMA)  
  - Model diagnostics and validation  
  - Forecast generation and comparison  

The notebook is written to be readable by both technical and non-technical audiences, with explanations provided alongside code, charts, and outputs.

---

## Dataset Overview

The dataset consists of **publicly available TSA passenger screening volumes**. Each observation represents the total number of passengers screened on a given day.

Key characteristics include:

- Daily passenger counts aggregated to monthly totals  
- Strong seasonal travel patterns  
- Significant disruptions during the COVID-19 period  
- Clear recovery and growth trends post-disruption  

The data captures both predictable demand cycles and periods of extreme volatility.

---

## Key Takeaways

- **Passenger demand is highly seasonal and predictable:** TSA volumes show consistent monthly patterns outside of extraordinary events.  
- **Validation strategy matters:** Models that perform well on a single holdout period may not be robust under real-world volatility.  
- **Manual ARIMA models proved more stable:** Carefully specified ARIMA models outperformed automated approaches when evaluated using rolling-origin validation.  
- **Forecasts are most valuable when tied to decisions:** Translating passenger forecasts into workforce planning context significantly increases their practical usefulness.  
- **Time series methods remain powerful:** Classical forecasting techniques can provide reliable, interpretable insights when applied thoughtfully.

---

## Notes

- This project was completed entirely as part of the USD Applied Data Science program.  
- All data used is publicly available.  
- Reports and presentations associated with this project are available upon request.

---
