# 📊 Telecom Customer Churn Prediction

## 👋 Overview

This project focuses on predicting whether a telecom customer will churn using machine learning.

The goal is not just prediction, but understanding why customers leave and identifying key business drivers behind churn.

---

## 📁 Dataset

- 7,043 telecom customers
- Each row represents one customer
- Target variable: `Churn (Yes/No)`

### Features:
- Contract type  
- Tenure  
- Monthly charges  
- Total charges  
- Payment method  
- Internet service details  

---

## 🔍 Exploratory Data Analysis (Key Insights)

- Customers with **month-to-month contracts** have the highest churn rate  
- Customers with **low tenure** are more likely to churn  
- Customers using **electronic check** payment method churn more  
- Higher **monthly charges** slightly increase churn probability  

---

## 📊 Visual Insights

### Churn Distribution
![Churn Distribution](images/churn_distribution.png)

### Tenure vs Churn
![Tenure vs Churn](images/tenure_vs_churn.png)

### Monthly Charges vs Churn
![Monthly Charges vs Churn](images/monthly_charges_vs_churn.png)

### Contract Type vs Churn
![Contract Type vs Churn](images/contract_vs_churn.png)

### Payment Method vs Churn
![Payment Method vs Churn](images/payment_method_vs_churn.png)

---

## ⚙️ Data Preprocessing

- Handled missing values in `TotalCharges`
- Converted `TotalCharges` to numeric
- Removed `customerID` (non-informative column)
- Applied one-hot encoding for categorical variables
- Converted target variable (Yes → 1, No → 0)

---

## 🤖 Model Building

- Model used: Logistic Regression  
- Train-test split: 80/20  
- Model trained on processed dataset  

---

## 📈 Model Performance

- Accuracy: ~82%  
- Recall (Churn class): ~60%  
- Precision (Churn class): ~68%  

### Key Insight:
Model performs better at predicting customers who stay than those who churn, which is common in imbalanced datasets.

---

## 🧠 Key Learnings

- Data cleaning is critical before modeling  
- Business understanding is more important than algorithm selection  
- Contract type and tenure are the strongest churn indicators  
- Recall is more important than accuracy in churn problems  

---

## 💼 Business Impact

This model helps telecom companies:

- Identify customers at risk of leaving  
- Take proactive retention actions  
- Reduce churn-related revenue loss  
- Improve customer retention strategy  

---

## 📊 Model Insights

Top churn drivers:
- Contract type  
- Tenure  
- Monthly charges  
- Payment method  

---

## 🛠 Tools Used

- Python  
- Pandas  
- NumPy  
- Scikit-learn  
- Matplotlib  
- Seaborn  

---

## 🚀 Future Improvements

- Try advanced models (Random Forest / XGBoost)  
- Handle class imbalance (SMOTE / class weights)  
- Tune decision threshold for better recall  
- Deploy model using Streamlit  

---

## 📌 Conclusion

This project demonstrates how data can be used to understand customer behavior and build predictive models that support business decisions.
