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

### Tenure vs Churn
<img width="600" height="400" alt="image" src="https://github.com/user-attachments/assets/15adf0b2-ea17-4839-a8d9-72132b41a8e8" />


### Monthly Charges vs Churn
<img width="600" height="400" alt="image" src="https://github.com/user-attachments/assets/dbe0fbb8-b260-4c4d-9565-3266b66afcaf" />


### Contract Type vs Churn
| Churn | Month-to-month | One year | Two year |
|------|----------------|----------|----------|
| No   | 0.429          | 0.253    | 0.318    |
| Yes  | 0.886          | 0.089    | 0.026    |

### Payment Method vs Churn
| Churn | Bank Transfer | Credit Card | Electronic Check | Mailed Check |
|------|--------------|-------------|------------------|--------------|
| No   | 0.249        | 0.249       | 0.250            | 0.252        |
| Yes  | 0.138        | 0.124       | 0.573            | 0.165        |

### Top Factors Driving Customer Churn
<img width="700" height="500" alt="image" src="https://github.com/user-attachments/assets/0b945628-44d4-473a-ae41-59f920624338" />


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
