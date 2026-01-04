# Forecasting Under Volatility: A Time-Series Approach to TSA Operations

This repository contains the final project deliverable for the graduate-level course  
**Applied Time Series Analysis (ADS 506)** in the M.S. in Applied Data Science program at the University of San Diego.

The assignment focused on applying classical time-series methods to a real operational problem, with an emphasis on **forecast robustness, validation under volatility, and translation of forecasts into actionable decisions**.

---

## Project Context

### Situation
The Transportation Security Administration (TSA) screens millions of passengers daily across U.S. airports. Passenger demand follows predictable seasonal patterns but is also subject to significant external shocks such as pandemics, government shutdowns, and extreme weather events. Historically, staffing decisions have been largely reactive, leading to inefficiencies, long wait times, and increased overtime costs.

### Task
The objective of this project was to determine whether TSA passenger demand can be forecast reliably despite volatility and to demonstrate how those forecasts could be used to support proactive workforce planning.

### Action
To address this problem, the project:
- Sourced publicly available TSA passenger screening data
- Aggregated daily passenger counts into monthly totals aligned with staffing decision cadence
- Conducted exploratory analysis to identify trends, seasonality, and structural breaks
- Evaluated multiple classical time-series models, including ETS and ARIMA
- Applied stationarity testing, differencing, and residual diagnostics
- Used rolling-origin cross-validation to assess model robustness across stable and volatile periods
- Translated passenger forecasts into workforce demand using operational throughput assumptions

### Result
The analysis showed that TSA passenger demand is highly predictable outside of extraordinary events and that **manually specified ARIMA models** outperform automated approaches when evaluated under rolling-origin cross-validation. Forecasts indicate continued growth in peak travel months, highlighting opportunities for TSA to move from reactive staffing to proactive, forecast-driven workforce planning.

---

## Problem Definition

**Problem:**  
How can TSA reliably forecast passenger demand under volatility and use those forecasts to improve staffing efficiency?

**Why it matters:**  
Inaccurate or reactive staffing leads to long wait times, increased overtime, wasted capacity during low-demand periods, and operational strain. Reliable forecasting enables better planning, cost control, and service-level stability.

**What time-series modeling solves:**  
Time-series models allow TSA to capture seasonality, trend, and recovery dynamics while explicitly modeling uncertainty and evaluating performance across historical shocks.

---

## Dataset Overview

- **Source:** TSA Passenger Volumes (public data)
- **Granularity:** Daily passenger counts
- **Time Range:** November 2019 – October 2025
- **Preprocessing:**
  - Aggregated daily data into monthly totals
  - Retained valid outliers related to holidays and COVID-19 disruption
  - Removed incomplete months from analysis

The dataset captures both predictable seasonal patterns and extreme volatility.

---

## What This Repository Contains

- A **fully documented analysis notebook** showing:
  - Data ingestion and preprocessing
  - Exploratory data analysis and STL decomposition
  - Model fitting and diagnostics
  - Forecast evaluation and comparison
  - Rolling-origin cross-validation
  - Workforce demand translation and visualization

> The written report and presentation were submitted separately for the course. This repository focuses on the analytical workflow and modeling output.

---

## Modeling Approach

The project evaluated several classical time-series models, including:

- Exponential Smoothing (ETS)
- Auto-ARIMA
- Manually specified ARIMA models

Model selection emphasized:
- Residual diagnostics over raw fit
- Stability across historical windows
- Performance under post-shock recovery periods
- Appropriateness for operational decision-making

Rolling-origin cross-validation was used to ensure robustness beyond a single holdout period.

---

## Key Findings

- **Validation strategy matters:** Models performing well on a single holdout period may fail under real-world volatility.
- **Manual ARIMA models proved more robust** than automated approaches across historical shocks.
- **Passenger demand is highly seasonal and predictable**, even after major disruptions.
- **Forecasts are significantly more valuable when translated into operational decisions**, such as staffing requirements.

---

## Why This Project Is Relevant

This project demonstrates how classical time-series techniques can be applied to real operational challenges and extended beyond forecasting into decision support.

The workflow reflects challenges commonly faced in:
- Operations and capacity planning
- Public-sector analytics
- Forecasting under uncertainty
- Workforce and resource optimization

---

## Notes

- This project was completed entirely as part of the USD Applied Data Science program.
- All data used is publicly available.
- Reports and presentations are available upon request.

---
