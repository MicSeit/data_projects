Telecom Customer Churn — End-to-End Predictive Analysis

Executive Summary
This project develops an end-to-end churn prediction pipeline for a telecommunications provider. Beyond predictive performance, the focus is on understanding churn behavior and translating model outputs into actionable retention insights.

Business Context
Customer churn is one of the primary revenue risks in subscription-based telecom services. Retention actions are costly, making accurate identification of high-risk customers essential.

The core business questions were:
- Which customers are likely to churn?
- Why are they churning?
- How can the business act on these insights?

Analytical Approach
The analysis followed a structured workflow:

1. Data Understanding
   - Churn distribution and class imbalance
   - Segmentation by tenure, contract type, and services

2. Feature Engineering
   - Encoding of categorical variables
   - Robust handling of missing and skewed values

3. Modeling Strategy
   - Baseline model for reference
   - Tree-based model optimized for recall
   - Evaluation focused on business-relevant metrics

Key Findings
- Contract structure and tenure dominate churn behavior
- Short-term contracts show significantly higher churn risk
- Model predictions enable targeted retention rather than blanket incentives

Outcome
The final model provides a scalable way to prioritize customers for retention campaigns, reducing unnecessary incentives while protecting revenue.

Tools & Technologies
Python, Pandas, NumPy, Matplotlib, Seaborn, Scikit-learn
