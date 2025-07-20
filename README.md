Credit Risk Analyzer 📊

A comprehensive data exploration and analysis project focused on identifying the factors influencing loan default risk using real-world financial data. This project includes data cleaning, feature engineering, EDA, correlation analysis, and insights useful for improving lending strategies. Built using Python, this analysis is also Power BI–ready for advanced dashboarding and business reporting.

🌐 Project Overview

Goal: Predict and explain loan default patterns by analyzing customer demographic and financial features in a structured credit dataset.

Dataset:

application_data.csv — 300K+ loan applications

previous_application.csv — historical applications

Target: TARGET column (1 = default, 0 = non-default)

🧪 Key Techniques Used

📋 Data Cleaning & Imputation

Dropped columns with >45% missing values

Imputed missing values using median, mode, or 'Unknown' based on skewness & feature type

🌍 Feature Engineering

Converted DAYS_BIRTH, DAYS_REGISTRATION, DAYS_ID_PUBLISH from days to years

Created annuity bands: low, medium, high, very high

Categorical encoding: Converted and visualized key features like OCCUPATION_TYPE, INCOME_TYPE, etc.

🔬 Exploratory Data Analysis

Visualized distributions using histograms, pie charts, countplots

Created bar plots comparing default vs non-default categories

⚖️ Statistical Testing

Applied Kolmogorov-Smirnov (KS) Test to identify features with significant distribution shifts

38+ variables found to differ between defaulters and non-defaulters

🔄 Correlation Analysis

Generated correlation matrices and heatmaps

Identified 28 pairs of features with correlation > 0.7

Built scatterplots to visualize multicollinearity

🔗 Data Merging

Merged application_data with previous_application on SK_ID_CURR

Analyzed trends across multiple loans for the same client

🌍 Dashboard Integration

Exported processed dataset for Power BI visualizations and real-time dashboarding

🔢 Tools & Libraries

Python (pandas, numpy, seaborn, matplotlib, scipy)

Statistical Testing: ks_2samp

Visualization: pie charts, histograms, countplots, barplots, heatmaps, scatterplots

Data Export: CSV format for Power BI

🌟 Key Insights

Males have a higher default ratio than females

Pensioners and highly educated individuals show better repayment performance

High annuity values and multiple previous loans are strong indicators of risk

High correlation found between loan amount and goods price

🔧 How to Use This Repo

To visualize data in Power BI:

Open previous_train.csv

Load into Power BI Desktop

Build visuals from cleaned fields like EXT_SOURCE_3, INCOME_TYPE, and TARGET

🏆 Future Improvements

Build machine learning model for risk prediction

Feature selection with RFE / SHAP for interpretability

Integrate dashboard directly with cloud data source

✨ Acknowledgements

Data source: Home Credit Default Risk - Kaggle

Notebook developed as part of upGrad Data Science program

Author: Venkatraman SContact: venkatraman8062@gmail.com
LinkedIn: linkedin.com/in/venkatraman8062
