# 🫀 HeartAttack Risk Predictor

A machine learning project for predicting the risk of a heart attack based on patient data.

## 📄 Project Overview

This project analyzes a heart-related dataset to build predictive models that determine whether a person is at risk of having a heart attack. Additionally, regression models were used to predict a person’s age, followed by age discretization for classification improvement.

## 🧠 Machine Learning Techniques Used

- **Linear Regression**  
- **Decision Tree Regressor & Classifier**
- **Random Forest**
- **Naive Bayes**
- **k-Nearest Neighbors (kNN)**
- **Logistic Regression**

Each model was trained with and without **normalization**. For classification tasks, **oversampling** was applied to handle class imbalance and compared to models without it.

## 🧪 Dataset Features

The dataset includes the following attributes:

- `age` – Age of the patient  
- `gender` – Gender  
- `cp` – Chest pain type (1–3)  
- `trbps` – Resting blood pressure  
- `chol` – Serum cholesterol  
- `fbs` – Fasting blood sugar  
- `thalach` – Max heart rate achieved  
- `oldpeak` – ST depression induced by exercise  
- `thall` – Result of thalassemia test  
- `exng` – Exercise-induced angina  
- `output` – Risk of heart attack (binary: 0 = No, 1 = Yes)

## ⚙️ Project Workflow

1. Data preprocessing: cleaning, handling missing values, feature selection  
2. Regression analysis for age prediction (with/without normalization)  
3. Age discretization into 3 categories:  
   - 29–40  
   - 41–55  
   - 56–77  
4. Classification using various models (with/without oversampling)  
5. Evaluation based on metrics such as Accuracy, ROC AUC, Precision, Recall, and F1-Score  

## 📊 Key Results

- ✅ **Random Forest Classifier** performed best:
  - Accuracy: ~82%
  - ROC AUC: 0.87
  - Balanced metrics across both classes

- 🧾 **Decision Trees (ID3, Gini)** performed similarly but showed signs of overfitting

- 📈 **Linear Classifier** had great recall on high-risk cases and benefited from normalization

- ⚠️ **Naive Bayes** and **kNN** underperformed, especially on minority classes

## 🧠 Insights

- **Normalization** significantly improved model performance  
- **Oversampling** helped with imbalance but caused overfitting in some models  
- **Discretizing age** improved classification accuracy  
- **Random Forest** proved to be the most stable and balanced model overall

## 👥 Authors

- Maksi krutinsky
- Roy Boker

## 📌 Conclusion

This project demonstrates how thoughtful preprocessing, feature engineering, and model selection can improve medical predictions using machine learning. Random Forest stands out as the most reliable model for classifying heart attack risk.
