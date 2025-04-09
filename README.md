# Post-Pandemic Analysis on Mortality Rate in Malaysia
This project investigates how mortality trends in Malaysia have changed following the COVID-19 pandemic, using statistical modeling to forecast future mortality rates. The goal is to provide insights for policy planning in areas such as healthcare, social security, and insurance.

## 📌 Objective
To analyze and forecast Malaysia’s mortality rates using statistical models, comparing pre-pandemic and post-pandemic trends. 

## 📁 Dataset
Data: [Central Mortality Rate]([url](https://www.dosm.gov.my/portal-main/release-content/abridged-life-tables-malaysia-2024)),[ Mid-Population Estimate
]([url](https://www.dosm.gov.my/portal-main/release-content/current-population-estimates-2024#:~:text=Overview&text=Malaysia's%20total%20population%20in%202024,cent%20to%200.7%20per%20cent.))

Years Covered: 2001–2022

Age Groups: (0, 1–4, 5–9, ..., 80+)

Covid-Adjusted Mortality: $nM'x = \frac{nD'x}{nPx}$

Source: Department of Statistics Malaysia (DoSM)

## 🔧 Tools & Models Used
| Programming/Software | Models | Packages | Skills | 
| --- | --- | --- | --- |
| R, Excel| Lee-Carter Model, ARIMA | ggplot2, fpp2, dplyr | Model fitting, residual analysis, time series forecasting, data analysis |

## 🛠️ Methodology
**1. Data Cleaning**
- Converted age-specific death and population counts into central mortality rates (nmx)
- Handled inconsistent age groupings and missing values
- Adjusted data to remove COVID-19-attributed deaths for comparison

**2. Data Visualization**
- Plotted mortality trends over time by age group
- Visualized effects of COVID-19 on overall and age-specific death rates

**3. Model Fitting**  
- Fitted the Lee-Carter on cleaned datasets
- Trained models on pre-pandemic data (e.g., 2001–2014), validated on 2015–2019
- Forecasted mortality up to 2035 under different assumptions (e.g., with/without COVID impact)

**4. Evaluation & Interpretation**
- Compared model performance based on forecast accuracy
- Analyzed the policy implications of projected mortality rates

## 🔑 Key Findings
- Significant spike in crude death rate in 2021 due to COVID-19.
- Mortality rates in older age groups, especially males, are most affected by COVID-19.
- Forecasted post-pandemic mortality rates are higher than pre-pandemic rates due to the excess death of COVID-19 but both declines over time.
