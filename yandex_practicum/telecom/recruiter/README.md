Telecom Customer Churn Prediction

Overview
This project analyzes customer churn for a telecommunications provider and builds a machine learning model to identify customers at high risk of leaving. The goal is to support data-driven retention strategies by identifying key churn drivers and predicting churn probability.

Business Problem
Customer churn directly impacts revenue and acquisition costs. The objective was to:
- Understand behavioral and contract-level drivers of churn
- Build a predictive model to flag high-risk customers
- Translate model outputs into actionable business insights

Data
- Customer demographic, contract, service usage, and billing data
- Binary churn target variable
- Several categorical and numerical predictors

Approach
1. Exploratory Data Analysis
   - Churn distribution and segmentation
   - Feature relationships and leakage checks

2. Feature Engineering
   - Encoding categorical variables
   - Handling missing values
   - Scaling numerical features

3. Modeling
   - Baseline model for comparison
   - Tree-based classification model
   - Evaluation using ROC-AUC and recall

Results
- Achieved strong predictive performance compared to baseline
- Identified contract type, tenure, and service usage as key churn drivers
- Model enables prioritization of retention efforts

Tools
- Python
- Pandas, NumPy
- Matplotlib, Seaborn
- Scikit-learn

Artifacts
- Full analysis notebook
- Source code and reproducible pipeline
