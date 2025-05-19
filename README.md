# Heart Disease Prediction

This repository contains a machine learning project that predicts the likelihood of heart disease based on patient medical data.

## Project Overview

Heart disease is a leading cause of death worldwide. Early prediction can help in timely diagnosis and treatment. This project uses various ML algorithms to analyze patient data and classify the risk of heart disease.




## Dataset

The dataset includes features such as age, gender, blood pressure, cholesterol levels, and other clinical measurements.

url
https://archive.ics.uci.edu/ml/machine-learning-databases/heart-disease/processed.cleveland.data

| Feature    | Description                                                          |
| ---------- | -------------------------------------------------------------------- |
| `age`      | Age of the patient (in years)                                        |
| `sex`      | Gender (1 = male; 0 = female)                                        |
| `cp`       | Chest pain type (0–3, where 0 = typical angina, 3 = asymptomatic)    |
| `trestbps` | Resting blood pressure (in mm Hg)                                    |
| `chol`     | Serum cholesterol in mg/dl                                           |
| `fbs`      | Fasting blood sugar > 120 mg/dl (1 = true; 0 = false)                |
| `restecg`  | Resting electrocardiographic results (0–2)                           |
| `thalach`  | Maximum heart rate achieved                                          |
| `exang`    | Exercise-induced angina (1 = yes; 0 = no)                            |
| `oldpeak`  | ST depression induced by exercise relative to rest                   |
| `slope`    | Slope of the peak exercise ST segment (0–2)                          |
| `ca`       | Number of major vessels (0–3) colored by fluoroscopy                 |
| `thal`     | Thalassemia (1 = normal; 2 = fixed defect; 3 = reversible defect)    |
| `target`   | Diagnosis of heart disease (0 = no disease; 1 = presence of disease) |


## Technologies Used

- Python  
- Scikit-learn  
- Pandas, NumPy  
- Matplotlib, Seaborn (for visualization)  
- Google colab notebook

##RESULT ANALYSIS
| **Algorithm**           | **Training Accuracy** | **Test Accuracy** | **Overall Accuracy** |
| ----------------------- | --------------------- | ----------------- | -------------------- |
| **Random Forest**       | 100.00%               | 90.16%            | 90.16%               |
| **SVM**                 | 90.08%                | 90.16%            | 90.16%               |
| **Naïve Bayes**         | 84.71%                | 83.61%            | 83.61%               |
| **Decision Tree**       | 100.00%               | 77.05%            | 77.05%               |
| **Logistic Regression** | 83.88%                | 88.52%            | 88.52%               |
| **K-Nearest Neighbors** | 83.88%                | 86.89%            | 86.89%               |
| **XGBoost**             | 100.00%               | 86.89%            | 86.89%               |


## Insights:
Both Random Forest and SVM achieved the highest test accuracy of 90.16%, demonstrating strong performance on unseen data.

Random Forest had a perfect training accuracy of 100.00%, indicating it learned the training data very well.

Decision Tree and XGBoost also showed 100% training accuracy, but lower generalization on test data, suggesting possible overfitting.

Naïve Bayes and KNN had lower overall accuracy, making them less ideal for deployment.

##  Final Model Selection
✅ Random Forest was selected as the final model for deployment because:

It achieved the highest test accuracy while also fitting the training data well.

It is robust to overfitting due to its ensemble nature.

It provides feature importance insights for medical interpretability.



