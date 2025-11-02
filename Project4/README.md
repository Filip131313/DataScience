# 🏦 Loan Default Prediction (Decision Tree vs Random Forest)

This project predicts whether a borrower will fully repay a loan using **Decision Tree** and **Random Forest** models.

---

## 📊 Dataset Overview

Each record represents a loan from **LendingClub.com**, containing borrower and loan details.  
**Target variable:** `not.fully.paid` (1 = not fully paid, 0 = fully paid)

During **Exploratory Data Analysis (EDA)**, I analyzed relationships between:
- `fico` score and `not.fully.paid`, `credit.policy`
- Purpose and `not.fully.paid`
- Interest rate (`int.rate`) and `fico` score'  
These visualizations helped understand general patterns before model training.

---

## 🧠 Model Results

| Model | Accuracy | Recall (unpaid loans) | F1-Score (unpaid loans) |
|--------|-----------|-----------------------|--------------------------|
| Decision Tree | 0.74 | **0.21** | **0.20** |
| Random Forest | **0.84** | 0.03 | 0.05 |

---

## ⚖️ Interpretation

- **Random Forest** performed better overall, predicting more accurately who **will repay** their loans.  
- **Decision Tree** performed slightly better at identifying borrowers who **won’t repay**.  
- Random Forest generalizes better, while Decision Tree tends to overfit but catches more risky cases.

---

## 💡 Feature Influence

Top influencing features:
- `installment`, `revol.bal`, `days.with.cr.line`, `revol.util`, `fico`

Borrowers with:
- **Low FICO scores**
- **High debt-to-income ratio (dti)**
- **High credit utilization (revol.util)**  
→ are more likely to **not fully repay**.

---

## 🧰 Libraries Used
`pandas`, `numpy`, `matplotlib`, `seaborn`, `scikit-learn`

---