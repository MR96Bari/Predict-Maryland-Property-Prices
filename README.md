# Maryland Housing Market Trends: Predicting Prices & Classifying Market Status

## 📌 Project Overview
This project analyzes Maryland's housing market data from **January 2022 to May 2024** to identify the key factors influencing **average sales prices** and to classify each county's market as **"Hot"** or **"Cold"**.  

Using statistical analysis and machine learning models, we:
- Built **linear regression models** to predict housing prices based on county, season, income, and market indicators.
- Applied **classification models** (Logistic Regression, Random Forest, KNN, etc.) to categorize market conditions.

## 🗂 Data Sources
- **Maryland Board of Realtors** – Monthly housing statistics (units sold, average prices, inventory, etc.)
- **U.S. Bureau of Economic Analysis (BEA)** – Personal income per capita
- **Maryland Office of Tourism** – Geographic region classifications

## 📊 Methods & Models
### 1. **Price Prediction**
- **Approach:** Multiple linear regression
- **Key predictors:** County, season, income
- **Best model:** LRMPrice_1 (explained variance ~ R² highest among tested models)
- **Performance:** ~12% RMSE and ~7% MAE relative to average price

### 2. **Market Classification**
- **Definition of "Hot" market:**  
  - Average sales price above state median  
  - Median days on market below state median
- **Best-performing model:** Random Forest (93% accuracy, perfect specificity)
- **Key predictors:** County, income

## 📈 Key Insights
- County-level data is more predictive of housing prices than regional-level data.
- Winter months correlate with lower sales prices.
- Income has a significant positive relationship with average sales prices.
- Random Forest models can accurately identify cold markets with zero false positives.

## 🛠 Technologies Used
- **R** for data cleaning, visualization, regression, and classification
- Libraries: `tidyverse`, `caret`, `randomForest`, `ggplot2`, etc.

## 📂 Repository Structure
