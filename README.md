Global Emissions and Population Analysis
Project Overview
This project examines the relationship between population trends, industrial activities, and emissions over time to understand factors contributing to climate change. We explore the impact of human activity on average global temperature using various machine learning models.

Contents
Data
Data Preprocessing
EDA
Modeling and Results

Data:
The dataset includes 31 features and 6965 records representing global metrics such as population, emissions, agricultural activities, and temperature over time.

Data Preprocessing
Feature Engineering: Created “Total Population” and “Total On-Farm Energy” features.
Scaling: Standardized features to handle outliers.
Multicollinearity Reduction: Removed highly collinear features using VIF.
EDA
Data cleaning
Population and Emissions: Urban population has a strong positive correlation with emissions.
Temperature Trends: Increase in temperature over time aligns with population growth and emissions.
Modeling and Results
Four models were tested: Linear Regression, Ridge, Lasso, and Random Forest. The Random Forest Regressor performed best, capturing non-linear relationships effectively.

Model	R² Score	RMSE
Linear Regression	0.025	0.51
Ridge Regression	0.025	0.51
Lasso Regression	0.024	0.51
Random Forest	0.428	0.39

Key Findings and Recommendations
Population and Emissions: Population growth, especially urbanization, correlates with increased emissions.
Industrial Impact: Emissions from food-related sectors are major contributors.
Random Forest Model: Recommended for future predictions due to its accuracy and handling of non-linear data.

Usage:
Clone the repository.
Install dependencies from requirements.txt.
Run analysis notebooks in the following order:
Analysis - Impact of agri activities on carbon emission.ipynb
Data preprocessing and model training.ipynb

Steps to install requirements.txt file
1. git clone <repository-url>
cd <repository-folder>

2. python -m venv venv
source venv/bin/activate    # On Windows: venv\Scripts\activate

3. pip install -r requirements.txt


Contributors: Xylon Dragner
Date: 11/11/2024