#  Telecom Customer Churn Prediction

A complete end-to-end Machine Learning project that predicts whether a telecom customer is likely to churn using supervised learning algorithms. The project includes data preprocessing, exploratory data analysis (EDA), feature engineering, model building, hyperparameter tuning, Explainable AI (SHAP & LIME), and business recommendations.

---

##  Project Overview

Customer churn is a major concern for telecom companies because retaining existing customers is significantly less expensive than acquiring new ones.

This project builds a predictive machine learning model to identify customers who are likely to leave the telecom service, enabling the business to take proactive retention measures.

---

##  Business Objective

Develop a machine learning solution capable of:

- Predicting customer churn
- Identifying major churn drivers
- Comparing multiple ML algorithms
- Explaining predictions using Explainable AI
- Providing actionable business recommendations

---

##  Project Structure

```
Telecom_Churn_Project/
│
├── data/
│   └── WA_Fn-UseC_-Telco-Customer-Churn.csv
│
├── notebooks/
│   └── Telecom_Customer_Churn.ipynb
│
├── reports/
│   ├── dataset_summary.xlsx
│   ├── dataset_audit.xlsx
│   ├── duplicate_records.csv
│   ├── missing_value_report.csv
│   ├── outlier_report.csv
│   ├── feature_engineering_report.xlsx
│   ├── encoding_report.csv
│   ├── correlation_matrix.csv
│   ├── vif_report.csv
│   ├── baseline_model_results.csv
│   ├── hyperparameter_results.csv
│   ├── feature_importance.csv
│   ├── model_comparison.csv
│   ├── business_understanding.docx
│   ├── eda_insights.docx
│   ├── business_recommendations.docx
│   └── lime_explanation.html
│
├── plots/
│   ├── churn_distribution.png
│   ├── correlation_heatmap.png
│   ├── feature_importance.png
│   ├── model_comparison.png
│   ├── shap_summary.png
│   └── ...
│
├── models/
│   ├── best_model.pkl
│   └── prediction_pipeline.pkl
│
└── README.md
```

---

#  Dataset

**Dataset:** Telco Customer Churn Dataset

The dataset contains customer demographic information, subscribed services, billing information, and customer churn status.

**Target Variable**

| Value | Meaning |
|--------|----------|
| Yes | Customer churned |
| No | Customer retained |

---

#  Technologies Used

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn
- XGBoost
- LightGBM
- SHAP
- LIME
- OpenPyXL
- Joblib

---

#  Exploratory Data Analysis

Performed comprehensive EDA including:

- Dataset summary
- Missing value analysis
- Duplicate analysis
- Outlier detection
- Numerical feature analysis
- Categorical feature analysis
- Correlation analysis
- VIF analysis
- Feature engineering

---

#  Feature Engineering

Created several business-driven features including:

- Avg_Monthly_Spend
- Long_Term_Customer
- Has_Multiple_Services
- Auto_Payment
- Electronic_Check
- Fiber_Internet
- High_Monthly_Charge
- Family_Customer
- Internet_User

---

#  Machine Learning Models

The following supervised learning algorithms were implemented:

- Logistic Regression
- Decision Tree
- Random Forest
- K-Nearest Neighbors (KNN)
- Support Vector Machine (SVM)
- XGBoost
- LightGBM

Each model was evaluated using:

- Accuracy
- Precision
- Recall
- F1 Score
- ROC-AUC

Hyperparameter tuning was performed using GridSearchCV.

---

#  Explainable AI

Model predictions were interpreted using:

### SHAP

- Global feature importance
- Model explainability
- Feature impact visualization

### LIME

- Local explanation for individual customer predictions
- Identification of key features influencing churn

---

#  Results

The tuned models achieved strong predictive performance.

## Final Model Performance

| Model | Accuracy | Precision | Recall | F1 Score | ROC-AUC |
|------|------:|------:|------:|------:|------:|
| Logistic Regression (Baseline) | 0.7402 | 0.5069 | **0.7861** | 0.6164 | **0.8465** |
| Logistic Regression (Tuned) | 0.7395 | 0.5060 | 0.7888 | 0.6165 | 0.8463 |
| AdaBoost (Baseline) | 0.7615 | 0.5358 | 0.7594 | 0.6283 | 0.8423 |
| XGBoost (Tuned) | 0.7779 | 0.5664 | 0.6952 | 0.6242 | 0.8420 |
| LightGBM (Tuned) | **0.7842** | **0.5866** | 0.6337 | 0.6093 | 0.8415 |

**Best Model (Based on ROC-AUC): Logistic Regression (Baseline)**

---

#  Business Insights

The analysis identified several major churn drivers:

- Month-to-Month contracts
- Short customer tenure
- High monthly charges
- Fiber Optic Internet
- Electronic Check payment method
- Lack of Online Security
- Lack of Technical Support

---

#  Deliverables

Generated project outputs include:

- Dataset Summary
- Dataset Audit
- Missing Value Report
- Duplicate Report
- Outlier Report
- EDA Insights
- Feature Engineering Report
- Correlation Matrix
- VIF Report
- Baseline Model Results
- Hyperparameter Results
- Feature Importance
- SHAP Summary Plot
- LIME Explanation
- Model Comparison
- Business Recommendations
- Saved Machine Learning Model

---

#  Future Improvements

- Deploy the model using Streamlit or Flask
- Real-time churn prediction API
- Automated model retraining
- Power BI dashboard integration
- Customer retention recommendation engine

---

#  Author

**Albin Karintholil Robert**

Master's in Data Science

---