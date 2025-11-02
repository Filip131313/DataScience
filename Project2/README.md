# 🛒 Ecommerce Customers: Yearly Spending Prediction

Predicting **yearly amount spent** by e-commerce customers using **Linear Regression**.

---

## 📊 Dataset

Features:

- Avg. Session Length  
- Time on App  
- Time on Website  
- Length of Membership  

**Target:** Yearly Amount Spent

**EDA** included `jointplots`, `pairplots`, and `regression plots` to understand relationships.

---

## 🧠 Model & Results

- **Linear Regression** trained on 70% of data  
- **Coefficients:**

| Feature | Coefficient |
|---------|------------|
| Avg. Session Length | 25.98 |
| Time on App         | 38.59 |
| Time on Website     | 0.19 |
| Length of Membership| 61.28 |

**Intercept:** -1047.93

- **Evaluation:**  
  - MAE, MSE, RMSE  
  - Explained variance score  
  - Residuals checked via histogram

---

## 💡 Insights

Based on the model, the **Time on App** is the most important feature for increasing yearly spending per customer.  
- Focusing on improving app engagement for new customers can increase revenue.  
- Additionally, encouraging users to become **members** (Length of Membership) further boosts spending.

---

## 🔧 Libraries

`pandas`, `numpy`, `matplotlib`, `seaborn`, `scikit-learn`

---
