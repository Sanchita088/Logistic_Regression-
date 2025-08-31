# Classification Models – Logistic Regression, Decision Tree & Random Forest

This project demonstrates how to build and evaluate **classification models** using three popular machine learning algorithms:

- Logistic Regression  
- Decision Tree  
- Random Forest  

The models are implemented in Python using **scikit-learn** and tested on the **Logistic Regression Dummy dataset** and **Car Evolution**.
# 📌 Logistic Regression – Classification Model

This project demonstrates **Logistic Regression**, a supervised machine learning algorithm used for **classification tasks**.  
It predicts the probability of a categorical dependent variable based on one or more independent variables.

---

## 🔎 What is Logistic Regression?

- Logistic Regression is used when the **target variable** is categorical (e.g., Yes/No, Pass/Fail, 0/1).  
- Instead of predicting exact values, it predicts the **probability** that a data point belongs to a certain class.  
- The output of Logistic Regression lies between **0 and 1**, using the **Sigmoid function**:  

\[
Sigmoid(z) = \frac{1}{1 + e^{-z}}
\]

---
# 🌳 Decision Tree & Random Forest – Car Evaluation Classification

This project demonstrates **Decision Tree** and **Random Forest** classification models using the **Car Evaluation Dataset**.  
Both models are implemented in Python with scikit-learn.  

---

## 🔍 What is Decision Tree?

- A **Decision Tree** is a flowchart-like structure where:  
  - Each **internal node** represents a feature condition  
  - Each **branch** represents an outcome of that condition  
  - Each **leaf node** represents a final class label  

- It splits the dataset into subsets based on **information gain** or **Gini index**.  
- Easy to interpret, but prone to **overfitting**.


---

## 🔍 What is Random Forest?

- **Random Forest** is an **ensemble method** that builds multiple Decision Trees and combines their predictions.  
- It reduces **overfitting** and improves **accuracy** compared to a single Decision Tree.  
- Final prediction is based on **majority voting** from all trees.

📌 Example:  
- Tree1 → acc  
- Tree2 → vgood  
- Tree3 → acc  
Final prediction → **acc** (majority vote)

---

## 📊 Car Evaluation Dataset

- **Source:** UCI Machine Learning Repository  
- **Features:**
  1. buying: vhigh, high, med, low  
  2. maint: vhigh, high, med, low  
  3. doors: 2, 3, 4, 5more  
  4. persons: 2, 4, more  
  5. lug_boot: small, med, big  
  6. safety: low, med, high  

- **Target Variable:**  
  - unacc, acc, good, vgood  


---

## 🚀 Steps in the Project

1. **Load Dataset**  
   Import dataset (`car_evaluation.csv`).  

2. **Preprocessing**  
   Encode categorical variables using `OrdinalEncoder` / `LabelEncoder`.  

3. **Train-Test Split**  
   Split dataset into 80% training and 20% testing.  

4. **Decision Tree Model**  
   ```python
   from sklearn.tree import DecisionTreeClassifier
   model = DecisionTreeClassifier(random_state=42)
   model.fit(X_train, y_train)

5. ```python
    from sklearn.ensemble import RandomForestClassifier
    model = RandomForestClassifier(n_estimators=100, random_state=42)
    model.fit(X_train, y_train)
6. Evaluation
   Compare both models using accuracy and classification report.




🚀 About Me
   Sanchita Dwivedi
🎓 M.Tech AIML Student | Python & ML Enthusiast

