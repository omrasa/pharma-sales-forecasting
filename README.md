# Pharmaceutical Sales Forecasting

## Overview
Time-series analysis and forecasting of monthly pharmaceutical drug sales 
using 17 years of historical data. Built a SARIMA model to predict future 
sales with 88.3% accuracy.

**Dataset:** Monthly drug sales 1991–2008 (204 data points)  
**Tools:** Python · Pandas · NumPy · Matplotlib · Statsmodels  

---

## Key Findings

- **January is peak sales month** — consistently 40% above annual average
- **Strong upward trend** across 17 years — sales grew from ~3.5 to ~25 units/month
- **SARIMA model achieved 88.3% accuracy** on 24 months of unseen data
- **Mean absolute error of 2.63 units/month** on a scale of 2.8–29.7

---

## Methods

**Exploratory Analysis:** Identified upward trend and strong seasonal pattern 
by visualising monthly averages across all years.

**Train/Test Split:** First 180 months used for training, last 24 months 
held out for model validation.

**SARIMA Model:** Seasonal AutoRegressive Integrated Moving Average with 
12-month seasonal cycle — standard approach for pharmaceutical demand 
forecasting.

**Validation:** Predictions compared against actual held-out data using 
Mean Absolute Error and percentage accuracy.

---

## Results

| Metric | Value |
|---|---|
| Training period | 1991–2006 (180 months) |
| Test period | 2006–2008 (24 months) |
| Mean Absolute Error | 2.63 |
| Forecast accuracy | 88.3% |
| Peak sales month | January |

---

## How to Run

```bash
git clone https://github.com/omrasa/pharma-sales-forecasting
cd pharma-sales-forecasting
pip install -r requirements.txt
jupyter notebook notebooks/
```

---

## Background

This project demonstrates time-series forecasting techniques applied to 
pharmaceutical commercial data — directly relevant to demand planning, 
inventory management, and sales operations roles in the pharma industry.