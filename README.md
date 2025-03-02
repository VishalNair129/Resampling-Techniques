# 🚗 Seatbelt Laws and Driver Fatalities: A Resampling-Based Analysis

This repository contains an analysis of **driver fatalities in Great Britain (1969-1984)** using **resampling techniques**. The study leverages **permutation tests, non-parametric bootstrapping, and regression modeling** to evaluate the impact of **seatbelt laws, seasonal trends, and economic factors** on road safety.

## 📌 Project Overview
The study is based on the **Seatbelts** dataset, which records monthly road accident statistics in Great Britain from **January 1969 to December 1984**. The dataset includes key variables such as:
- **DriversKilled**: Monthly count of driver fatalities.
- **kms**: Total distance driven (in thousands of kilometers).
- **PetrolPrice**: Fuel price per unit.
- **law**: Indicator of whether the **1983 seatbelt law** was in effect (0 = before, 1 = after).
- **Front/Rear Passenger Fatalities**: Count of fatalities by seating position.

The goal is to apply **statistical resampling** to assess:
✔ The impact of **seatbelt laws** on driver fatalities.  
✔ The presence of **seasonal patterns** in accident rates.  
✔ Differences in **front vs. rear passenger fatalities**.  
✔ The relationship between **fuel prices, distance driven, and road fatalities**.  

## 🔬 Methodology
To ensure statistical robustness, we apply:
1. **Permutation Tests**:  
   - Assess the effect of **seatbelt laws** by randomly shuffling fatalities and recomputing test statistics.  
   - Evaluate differences in **front vs. rear passenger fatalities** with randomized data distributions.

2. **Two-Way ANOVA**:  
   - Analyze the combined effect of **seasonality** and **seatbelt laws** on fatalities.  
   - Validate results using **permutation-based F-tests**.

3. **Multiple Linear Regression**:  
   - Model the impact of **kilometers driven** and **fuel prices** on fatalities.  
   - Apply **bootstrap-t confidence intervals** to validate regression coefficients.

## 📊 Results and Observations
- **Seatbelt Law Effect**: Fatalities **significantly decreased** post-law (p < 0.05).
- **Seasonality**: Higher accident rates were observed in **winter months**.
- **Front vs. Rear Fatalities**: Front-seat passengers were at **greater risk** of fatality than rear-seat passengers (p < 0.01).
- **Economic Factors**: **Higher fuel prices** were associated with **fewer fatalities**, indicating a possible **demand elasticity effect**.

## ⚠️ Limitations
- The dataset covers **only 1969-1984**, excluding modern safety measures.
- Confounding variables like **weather conditions** or **law enforcement efforts** were not explicitly controlled.
- The analysis assumes **stationarity in driver behavior**, which may not hold across decades.

## 🔮 Future Work
- Apply **time-series forecasting** models for **accident risk prediction**.
- Incorporate **machine learning approaches** for enhanced safety analysis.
- Compare with **modern datasets** to assess long-term road safety trends.

