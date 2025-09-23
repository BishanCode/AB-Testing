#  A/B Testing – Ecommerce Landing Page

##  Project Overview
This project analyzes an **A/B test** for an e-commerce landing page.  
The goal was to determine whether the **new landing page (treatment)** improved conversion rates compared to the **old landing page (control)**.  

Dataset: [Kaggle – Ecommerce A/B Testing 2022](https://www.kaggle.com/datasets/putdejudomthai/ecommerce-ab-testing-2022-dataset1/data)  
Date Accessed: 12th September 2025  

---

##  Workflow

1. **Data Preparation**
   - Merged user data with country info
   - Removed duplicates and inconsistent rows
   - Verified group assignments (control → old page, treatment → new page)

2. **Exploratory Data Analysis**
   - Checked group balance (≈50/50 split)
   - Checked country distribution across groups
   - Calculated overall and country-level conversion rates

3. **Hypothesis Testing**
   - Two-proportion z-test for conversion difference
   - Confidence intervals for conversion rates
   - Tested for balance using chi-square
   - Logistic regression (optional) adjusting for country

4. **Visualisation**
   - Conversion rate comparison (control vs treatment)
   - Conversion by country
   - Funnel-style summary

5. **Dashboard (Power BI)**
   - KPIs: conversion rate, absolute lift, p-value
   - Country-level breakdown
   - Filters for interactivity

---

## 📊 Key Results
- **Control conversion rate:** 12.04%  
- **Treatment conversion rate:** 11.88%  
- **Absolute lift:** -0.16%  
- **Relative lift:** -1.30%  
- **p-value:** 0.1892  
- **95% CI for lift:** [-0.39%, +0.07%]  


➡️ **Decision:** The new landing page did *not* produce a statistically significant improvement. Rollout not recommended at this time.  

---

##  Tech Stack
- **Python**: pandas, numpy, statsmodels, scipy, seaborn, matplotlib  
- **Power BI**: dashboard visualization  
- **Jupyter Notebook**: analysis workflow  

---

