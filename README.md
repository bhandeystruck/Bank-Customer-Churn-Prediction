
# 🏦 Bank Customer Churn Prediction

This is an end-to-end machine learning project to predict customer churn using a real-world inspired bank dataset. The project focuses on understanding why customers leave the bank and building an interpretable logistic regression model to identify customers at risk of churning.

---

## 📌 Project Highlights

- 🔍 Exploratory Data Analysis (EDA)
- 🧼 Data Cleaning & Outlier Detection
- 🧠 Feature Engineering (Engagement score, loyalty ratio, etc.)
- 🚩 Outlier & Underbanked Flags
- 📊 Logistic Regression Model with Balanced Class Weights
- 📈 Model Evaluation: Precision, Recall, F1, ROC AUC
- 💬 Business Insights and Churn Strategy Recommendations

---

## 📂 Dataset Overview

The dataset includes the following features:

- Demographics: `age`, `gender`, `country`
- Bank interaction: `tenure`, `balance`, `estimated_salary`
- Product usage: `num_of_products`, `has_credit_card`, `is_active_member`
- Engineered features: `engagement_score`, `balance_salary_ratio`, `loyalty_score`, etc.
- Target: `churn` (0 = stayed, 1 = churned)

---

## 🧠 Feature Engineering

Created several insightful features such as:

- `engagement_score` = activity + credit card usage + product count
- `loyalty_score` = tenure / (age + 1)
- `balance_salary_ratio` = balance / (estimated_salary + 1)
- Flags for high-value customers, underbanked users, and low credit score holders

---

## 🤖 Model: Logistic Regression

- Trained with and without class balancing
- Balanced model improved recall for churners from 31% ➜ 73%
- ROC AUC = **0.81** (strong discriminatory power)

---

## 📊 Evaluation

- Confusion matrix and classification report used to assess performance
- Feature importances extracted for interpretability
- Model and scaler saved for future predictions

---

## 🔮 What's Next

- Train Random Forest and XGBoost for performance comparison
- Visualize SHAP values for model transparency
- Build a Streamlit app or dashboard
- Generate customer churn probability scores and prioritize high-risk users

---

## 🚀 Run Locally

1. Clone the repo  
```bash
git clone https://github.com/your-username/bank-churn-prediction.git
```

2. Install requirements  
```bash
pip install -r requirements.txt
```

3. Run the notebook or use the saved model for predictions

---

## 📬 Contact

Created by [Your Name] · [your.email@example.com] · [LinkedIn/GitHub profile]

---

## 📄 License

This project is open source and available under the [MIT License](LICENSE).
