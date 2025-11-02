# 🌸 Iris Species Classification with SVM

This project classifies Iris flower species using **Support Vector Machines (SVM)** and **GridSearchCV** for hyperparameter tuning.

---

## 📊 Dataset Overview

The dataset contains 150 samples of three Iris species: `setosa`, `versicolor`, and `virginica`.  
Features include:
- `sepal_length`
- `sepal_width`
- `petal_length`
- `petal_width`  

**Target variable:** `species` (categorical: setosa, versicolor, virginica)

During **Exploratory Data Analysis (EDA)**:
- Pairplots were created to visualize relationships between features per species.
- Kernel density estimation (KDE) plots were used to examine distributions of `setosa`.

---

## 🧠 Model Approach

- Split the data into training and test sets (70% train / 30% test).  
- Trained a **Support Vector Classifier (SVC)**.  
- Applied **GridSearchCV** to find the best combination of `C` and `gamma` for improved performance.

---

## 📈 Model Results

**Confusion Matrix and Classification Report (after GridSearchCV):**  

| Species      | Precision | Recall | F1-Score | Support |
|--------------|-----------|--------|----------|---------|
| setosa       | 1.00      | 1.00   | 1.00     | 12      |
| versicolor   | 1.00      | 1.00   | 1.00     | 15      |
| virginica    | 1.00      | 1.00   | 1.00     | 18      |

**Overall Accuracy:** 1.00  

The model perfectly classifies all three species on the test set.

---

## 💡 Key Points

- SVM performed very well with properly tuned hyperparameters (`C` and `gamma`).  
- Pairplots and KDE plots helped understand feature distributions and separability between species.  

---

## 🧰 Libraries Used

`pandas`, `seaborn`, `matplotlib`, `scikit-learn`

---