This Repository is for my Capstone Project about Machine Learning. The main objective of this project is identifying the churn rate of a Telco Company and what can be done about it.

A. Business Understanding
Customer churn represents a significant loss for telecommunication companies, as acquiring new customers is far more expensive than retaining existing ones.
This project addresses the following business goals:
- Predict which customers are likely to churn.
- Identify factors that influence churn.
- Recommend strategies for customer retention.
  
==Project Workflow==
1. Business Understanding
   - Define objectives and translate them into a data science problem.
3. Data Understanding
   - Perform exploratory data analysis (EDA) on Telco customer data.
   - Identify churn distribution and correlations with features.
5. Data Preparation
   - Handle missing values and duplicates.
   - Encode categorical features and scale numerical features.
   - Split data into training and testing sets with stratification.
7. Modeling
   - Logistic Regression (baseline + tuned).
   - Random Forest.
   - XGBoost (tuned with RandomizedSearchCV).
9. Evaluation Metrics
   - Compare models using metrics such as Accuracy, Precision, Recall, F1-score, and ROC-AUC.
   - Select the best model for business needs.

The selected model for this specific problem is Logistic Regression. The reason behind this:
- It achieved a high recall rate (80%) for churn customers.
- It demonstrated a high ROC-AUC (0.84), meaning strong ability to discriminate between churn and non-churn.
- It provides interpretable coefficients, enabling clear insights into churn drivers.

Insights :
- Customers on month-to-month contracts are significantly more likely to churn.
- Higher monthly charges increase the risk of churn.
- Fiber optic customers churn at higher rates than DSL customers.
- Customers with longer tenure or two-year contracts are less likely to churn.
- Use of add-on services (Online Security, Backup, Tech Support) decreases churn likelihood.

Recommendation :
- Promote long-term contracts (offer incentives to move customers from monthly to yearly/two-year contracts).
- Bundle services to provide better value for high-charge customers.
- Improve fiber optic service quality and customer support.
- Encourage adoption of add-on services (free trials, loyalty rewards).
- Reward long-tenure customers through loyalty programs.
