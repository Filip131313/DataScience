# Ad Click Prediction Project

## Project Overview
This project aims to predict whether a user will click on an online advertisement based on their personal attributes and internet usage data. It is a **binary classification problem** where we use **Logistic Regression** to make predictions.

The project provides insights into which users are more likely to click on ads, helping businesses optimize their ad targeting strategies.

---

## Key Insights
- The **average age** of users who click on ads is around **40 years old**.  
- **Females** are more likely to click on ads compared to males.  
- **Marketing focus:** Target **females around 40 years old** for better engagement and higher click-through rates.  
- Other factors like **Area Income** and **Daily Time Spent on Site** also influence click probability but less strongly.

---

## Dataset
The dataset contains the following features for each user:

- **Age** – Age of the user  
- **Area Income** – Income of the area the user lives in  
- **Daily Time Spent on Site** – Average daily time spent on the website  
- **Daily Internet Usage** – Average daily time spent on the internet  
- **Male** – Gender of the user (`0 = Female`, `1 = Male`)  
- **Clicked on Ad** – Target variable (`0 = Did not click`, `1 = Clicked`)  

**Note:** Initially, any **null values** in the dataset were removed before analysis.

---

## Steps Performed

### 1. Data Preprocessing
- Removed null values to clean the dataset.  
- Loaded the dataset from a **CSV file**.  
- Encoded categorical variables (e.g., Male) into numeric format using one-hot encoding.  
- Split the dataset into **training and testing sets** using `train_test_split`.

### 2. Modeling
- Trained a **Logistic Regression** model to predict `Clicked on Ad` using other features.  
- Set `max_iter=1000` to ensure convergence of the model.  

### 3. Model Evaluation
Predictions were generated on the test set and evaluated using:

- **Accuracy** – Overall correctness of predictions.  
- **Precision** – Proportion of predicted clicks that were actual clicks.  
- **Recall** – Proportion of actual clicks that were correctly predicted.  
- **F1-score** – Harmonic mean of precision and recall.  
- **Confusion Matrix** – Shows **true positives, false positives, true negatives, and false negatives**.  


- **Intercept:** 25.3374  
- This shows that **Age** and **Gender** have the most significant impact on predicting ad clicks.  
- Older users and females are more likely to click on ads.

---

## Tools & Libraries Used
- **Python** – Programming language  
- **Pandas** & **NumPy** – Data manipulation and numerical computation  
- **Scikit-learn** – Machine learning (Logistic Regression)  
- **Seaborn** & **Matplotlib** – Data visualization  

---

## Conclusion
This Logistic Regression model successfully predicts ad clicks with high accuracy. Businesses can use these insights to optimize advertising campaigns and focus on the most promising user segments.