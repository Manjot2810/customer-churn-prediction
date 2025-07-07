# 🔍 Customer Churn Prediction

This project aims to predict customer churn using machine learning models on the Telco Customer Churn dataset. It includes data cleaning, exploratory data analysis (EDA), feature engineering, and training of classification models like **Logistic Regression**, **Random Forest**, and **XGBoost**.

---

## 📂 Dataset

- **Source:** [Telco Customer Churn](https://www.kaggle.com/blastchar/telco-customer-churn)
- **Rows:** ~7,000
- **Target Variable:** `Churn` (1 = Customer left, 0 = Customer stayed)

---

## 📊 Features Used

- Demographics: `gender`, `SeniorCitizen`, `Partner`, `Dependents`
- Service details: `InternetService`, `OnlineSecurity`, `TechSupport`, etc.
- Account info: `Contract`, `PaymentMethod`, `MonthlyCharges`, `TotalCharges`

---

## 🧠 Models Used

| Model               | Accuracy | Recall | ROC-AUC |
|--------------------|----------|--------|---------|
| Logistic Regression| ✅       | ✅     | ✅      |
| Random Forest       | ✅       | ✅     | ✅      |
| XGBoost             | ✅       | ✅     | ✅      |

(*Actual numbers depend on the run; check the notebook for detailed scores.*)

---

## 🛠️ Tech Stack

- Python 3.x
- pandas, numpy
- seaborn, matplotlib
- scikit-learn
- xgboost

---

## 📈 Workflow

1. **Data Preprocessing**
   - Handle missing values in `TotalCharges`
   - Encode categorical variables
   - Scale features

2. **EDA**
   - Churn distribution
   - Feature correlation
   - Service-wise churn analysis

3. **Modeling**
   - Logistic Regression
   - Random Forest
   - XGBoost

4. **Evaluation**
   - Accuracy
   - Recall (for imbalanced data importance)
   - ROC-AUC and ROC curves

---

## ▶️ How to Run

```bash
# Clone the repo
git clone https://github.com/yourusername/customer-churn-prediction.git
cd customer-churn-prediction

# (Optional) Create virtual environment
python -m venv venv
source venv/bin/activate  # or venv\Scripts\activate on Windows

# Install dependencies
pip install -r requirements.txt

# Run Jupyter Notebook or script
jupyter notebook churn_prediction.ipynb
