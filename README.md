# 📉 Customer Churn Analyzer

Predicting customer churn is critical for telecom and subscription-based businesses. This project uses machine learning to identify customers at risk of leaving, enabling proactive retention strategies.

---

## 🧠 Problem Statement

Customer churn leads to revenue loss and increased acquisition costs. By analyzing customer behavior and service interactions, we aim to predict churn and support data-driven retention efforts.

---

## 📦 Dataset Overview

- **Source**: `churn_sample.csv`
- **Rows**: 1002 customers
- **Features**:
  - `Contract`, `Support Calls`, `Monthly Bill`, `Payment Method`, `Billing Issues`
  - `DataStage GB`, `Tenure Months`, `AutoPay`
  - `Churn` (target variable)

---

## 🔍 Exploratory Data Analysis

- 📊 **Churn Distribution**: Pie chart with churn percentages
- 📈 **Monthly Bill vs Churn**: Box + swarm plot reveals billing trends
- 🎻 **Support Calls vs Churn**: Violin plot shows interaction intensity
- 📌 **Contract Type Impact**: Bar chart highlights churn-prone plans
- 🔗 **Correlation Matrix**: Heatmap of feature relationships

---

## ⚙️ Model Building

- **Algorithm**: Logistic Regression
- **Preprocessing**: Label encoding for categorical features
- **Split**: 70% training / 30% testing
- **Evaluation**:
  - Confusion matrix
  - Classification report
  - F1 score

---

## 📊 Feature Importance

Top churn indicators based on model coefficients:
- High number of support calls
- Monthly contracts
- Lower tenure and absence of AutoPay

---


## 🔮 Prediction Example

```python
Input:
Contract: Monthly
Support Calls: 6
Monthly Bill: ₹110

Output:
Predicted Churn: Yes


▶️ How to Run this project.
Install dependencies

bash
pip install -r requirements.txt

Launch the notebook Open Customer Churn Analyzer.ipynb in Jupyter or upload to Google Colab.

Run all cells sequentially The notebook covers data loading, EDA, model training, evaluation, and prediction.

Test with custom input Modify the final cell to predict churn for new customer data.

📌 Key Insights
Customers with monthly contracts and frequent support calls are more likely to churn.
AutoPay and longer tenure reduce churn risk.
Model accuracy is moderate (~54%), suggesting room for improvement via feature engineering or alternate classifiers.

🚀 Future Enhancements
Try decision tree or ensemble models
Add hyperparameter tuning
Integrate SHAP for model explain ability
Deploy as a web app for real-time churn prediction


🙋 Author
Nandni Jaiswal.
B.S. Computer Science & Data Analytics, IIT Patna
Roll no - 2312res965

