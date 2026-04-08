# 🌍 Global Inflation Analysis & Prediction

## Project Overview
This project analyzes global inflation trends from 1960 to 2024 and builds predictive models to forecast inflation at the country level. Using historical World Bank data, the project explores how inflation varies across countries and over time, identifies outliers and extreme events, and develops machine learning models to predict future inflation trends.

---

## Key Objectives
- Analyze global and country-specific inflation trends.  
- Identify countries with extreme inflation events.  
- Build predictive models to forecast inflation using historical data.  
- Provide actionable insights for economic and business decisions.

---

## Tools & Technologies
- **Python:** Pandas, NumPy, Matplotlib, Seaborn, Scikit-learn  
- **SQL:** PostgreSQL for business question analysis  
- **Machine Learning:** Linear Regression, Random Forest Regression  
- **Visualization:** Line plots, bar charts, histograms, boxplots  

---

## Project Steps

### 1. Data Cleaning & Preprocessing
- Removed missing values and extreme outliers.  
- Reshaped dataset into a long format.  
- Converted year to numeric type.  

### 2. Exploratory Data Analysis (EDA)
- Visualized top 10 countries by average inflation.  
- Analyzed global inflation trends over years.  
- Examined distribution of inflation values using histograms and boxplots.  
- Studied country-specific trends to identify variability and outliers.  

### 3. Business Analysis Using SQL
- Connected dataset to PostgreSQL.  
- Answered business questions like highest inflation countries, year-wise trends, and extreme inflation events.  
- Validated insights observed during EDA.  

### 4. Feature Engineering
- Encoded `Country Name` as numeric for modeling.  
- Applied log transformation on `Inflation` to reduce skewness from extreme values.  

### 5. Modeling
#### Linear Regression (Baseline)
- Used `Year` as the only feature.  
- R² ≈ 0.04 — indicated poor performance, year alone is insufficient.  

#### Random Forest Regression
- Used `Year` and `Country_encoded` as features with log-transformed `Inflation` as target.  
- R² ≈ 0.63 (log scale) — captured non-linear patterns and country-specific effects.  
- Mean Squared Error ≈ 0.335 (log scale).  

---

## Insights & Interpretation
- Extreme inflation spikes in certain countries indicate periods of economic instability.  
- Emerging economies showed rapid inflation growth, affecting purchasing power.  
- Long-term deflation in some countries could limit economic expansion.  
- Historical trends suggest potential future inflation risks in specific regions.  
- Both time and country-level factors significantly influence inflation patterns.

---

## Conclusion
This project demonstrates an end-to-end data science workflow: data cleaning, exploratory analysis, SQL business queries, feature engineering, modeling, and interpretation. Random Forest regression effectively captured complex, non-linear patterns and provided a moderately strong predictive model, making it valuable for economic and business decision-making.

---

## Future Work
- Incorporate additional macroeconomic indicators (GDP, CPI, unemployment).  
- Explore advanced models like Gradient Boosting or XGBoost.  
- Improve predictions for extreme inflation events.  
- Build interactive dashboards for monitoring trends in real time.  

