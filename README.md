# Sales Prediction Using Linear Regression

## Project Overview
This project builds a statistical model to predict company sales using multiple business drivers, including advertisement budget, store expansions, seasonal factors, and economic indicators. The objective is to uncover which features significantly influence sales performance and assess the effectiveness of a linear regression approach.

## Dataset
- Simulated marketing campaign data with 1,000 rows
- Features:
  - `advertisement_budget` (numeric)
  - `social_media_spend` (numeric)
  - `store_openings` (numeric)
  - `economic_index` (numeric)
  - `season` (categorical: Spring, Summer, Autumn, Winter)
  - `sales` (target variable)

## Preprocessing
- One-hot encoding applied to the `season` variable
- All features converted to numeric format
- Data split into X (features) and y (target)

## Model Summary
- Built an **OLS Linear Regression** model using `statsmodels`
- Key findings:
  - **Significant predictors:** `advertisement_budget`, `store_openings` (p < 0.01)
  - **Insignificant predictors:** `social_media_spend`, `economic_index`, season dummies
- **Model performance:**  
  - R² = 0.025 → indicates poor explanatory power

## Limitations
- Low R² suggests linear regression may not capture complex patterns
- Multicollinearity concerns (high condition number)
- Dataset lacks variables like product type, region, or discounts

## Tools Used
- Python: `pandas`, `statsmodels`, `matplotlib`, `seaborn`

## Project Files
- `sales_regression_analysis.ipynb`: Full analysis and model
- `marketing_campaign_data.csv`: Dataset
- `README.md`: Project documentation

## Author
Sakshi Gupta  
Data Analyst | Python | Regression | Statistics | Business Analytics  
New Delhi, India

