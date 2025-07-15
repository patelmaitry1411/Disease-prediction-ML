# Disease-prediction-ML
---

## Dataset Description

- **132 binary symptom columns**: e.g., `Symptom_1`, `Symptom_2`, ..., `Symptom_132`
- **Target**: Disease (41 possible classes like `Disease_1`, `Disease_2`, ..., `Disease_41`)
- **500 rows** of randomly generated patient symptom data

---

## Problem Statement

> Predict the disease based on selected symptoms using a machine learning classifier.

This project is designed for educational and prototyping purposes, showcasing how ML can be applied to healthcare data.

---

## Technologies Used

- **Python**
- **Pandas**
- **Scikit-learn**
- **RandomForestClassifier**
- **LabelEncoder**
- **Jupyter Notebook / Google Colab**

---

## How It Works

1. Load the dataset containing 132 symptoms and their corresponding disease.
2. Encode the disease labels using `LabelEncoder`.
3. Split the dataset into training and testing sets.
4. Train a **Random Forest Classifier**.
5. Input user symptoms (binary values) and predict the most likely disease.

---

## Sample Code Snippet

```python
model = RandomForestClassifier()
model.fit(X_train, y_train)
y_pred = model.predict(X_test)
accuracy_score(y_test, y_pred)
