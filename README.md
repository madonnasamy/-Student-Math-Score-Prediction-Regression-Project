# 🎓 Student Math Score Prediction using Regression

This project uses supervised machine learning techniques to predict students' math exam scores based on demographic and academic factors.

---

## 📌 Problem Statement

We aim to build a regression model that accurately predicts a student's **math score** based on:
- Gender
- Race/Ethnicity
- Parental level of education
- Lunch type
- Test preparation course
- Reading and Writing scores (optional)

---

## 📊 Dataset

- Source: [Kaggle – Student Performance Data](https://www.kaggle.com/datasets/spscientist/students-performance-in-exams)
- Size: 1000 rows
- Format: CSV file
- Target Variable: `math score`

---

## 🛠️ Preprocessing

- Label Encoding for categorical features:
  - `gender`, `lunch`, `test preparation course`
  - `parental level of education`, `race/ethnicity`
- No missing values
- Train-test split: 80% train, 20% test

---

## 🤖 Models Used

We tested and compared the following regression models:

| Model                    | MAE  | RMSE | R² Score |
|--------------------------|------|------|----------|
| **Linear Regression**     | 4.13 | 5.32 | **0.88** |
| Random Forest Regressor   | 4.68 | 6.05 | 0.85     |
| SVR (Support Vector)      | 5.81 | 8.62 | 0.69     |

> ✅ **Best model**: Linear Regression – simple and most effective on this dataset.

---

## 📦 Libraries Used

```python
pandas
numpy
scikit-learn
matplotlib
seaborn
