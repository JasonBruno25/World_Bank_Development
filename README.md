# World_Bank_Development
A Machine Learning project

# World Bank Development Data Dashboard

An interactive R flexdashboard analyzing global development trends (2000–2022) using six statistical learning methods. This project was completed for a graduate-level course (CMDA 4654) at Virginia Tech.

## Live Dashboard

> *The dashboard is an HTML file – download or view locally after rendering.* 
> *Need to add a live demo link but need to be hosted first.*

## Team Members

- **Matthew Pannell** – Multiple Regression, kNN Classification, Naive Bayes, dashboard formatting  
- **Jason Bruno Terceros** – Ridge Regression, Logistic Regression, Project Background page, dashboard formatting  
- **Porter Lin** – LOESS smoothing, dashboard formatting  

## Abstract

This dashboard analyzes socioeconomic and infrastructure indicators from the World Bank across multiple countries (2000–2022). We investigate distinct research questions using six different regression and classification techniques: Multiple Regression, Ridge Regression, LOESS smoothing, kNN Classification, Naive Bayes Classification, and Logistic Regression. The results are visualized through maps, plots, and professional tables, offering clear insight into global development patterns.

## Methods & Key Findings

| Method | Research Question | Key Result |
|--------|------------------|-------------|
| **Multiple Regression** | Predict GDP per capita from education, health expenditure, and urbanization | R² = 0.96 after log & sqrt transformations |
| **Ridge Regression** | Predict GDP from inflation, unemployment, exports, and capital formation | Optimal lambda via cross-validation; multicollinearity controlled |
| **LOESS (degree 1 & 2)** | Model GDP per capita trends over time for 6 countries | MSE varies by country; degree-2 often better but risk of overfitting |
| **kNN Classification** | Classify high/low internet usage from economic indicators | Best k = 7; accuracy = 90.4% |
| **Naive Bayes** | Classify high/low life expectancy from health, urban, electricity | Accuracy = 97.1% |
| **Logistic Regression** | Predict low life expectancy (<70 years) from unemployment, Gini, GDP | AUC = 0.951 |

## Data Source

- World Bank Open Data – World Development Indicators  
- Variables include: GDP per capita, Gini index, unemployment, inflation, exports, capital formation, life expectancy, school enrollment, health expenditure, population growth, electricity access, internet usage, mobile subscriptions, urban population.  
- Data range: 2000–2022  

## Repository Contents

- Project_1_Group_09.Rmd # R Markdown source for flexdashboard
- Global-Development-Dashboard.html # Self-contained interactive dashboard
- worldbank.csv # Raw data (if permitted to share)
- README.md # This file
