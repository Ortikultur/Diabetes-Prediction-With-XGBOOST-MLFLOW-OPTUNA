# Predicting Diabetes in Patients 

This project employs machine learning techniques to predict diabetes occurrence in patients using several features. Building  a model that accurately identifies diabetic patients, for early detection and treatment.

## Project Overview

1. **Dataset:** The dataset includes information about gender, age, hypertension, blood glucose levels, heart disease, smoking history,bmi, HbA1c (Hemoglobin A1c) level and diabetes status.
   
2. **Data Preprocessing:** The dataset underwent preprocessing steps such as encoding categorical variables, and scaling numerical features. A stratifiedKFold was performed for balanced class distribution.

4. **Model Selection:** I chose XGBoost as the machine learning model for predicting diabetes, considering its effectiveness in handling complex relationships in data.

5. **Evaluation Metrics:** The model's performance was assessed using ROC-AUC, precision, recall  and accuracy providing insights into its ability to classify diabetic and non-diabetic patients accurately.

6. **Hyperparameter Tuning:** To enhance the model's performance, I utilized Optuna for hyperparameter optimization. Optuna systematically explores hyperparameter spaces to find the optimal set of parameters for the XGBoost model.

## Results

After preprocessing, model training, and hyperparameter tuning, the following test set performance metrics were achieved:

- **ROC AUC Score:** 0.7645
- **Recall Score:** 0.8102
- **Accuracy Score:** 0.7431
- **Precision Score:** 0.5101
- **F1 Score:** 0.6260
- **F2 Score:** 0.7249

**Classification Report:**

           precision    recall  f1-score   support
       0       0.91      0.72      0.80      1035
       1       0.51      0.81      0.63       374

accuracy                           0.74      1409
                                   0.74      1409
macro avg 0.71 0.76 0.72 1409
weighted avg 0.81 0.74 0.76 1409

These results indicate that the XGBoost model performs reasonably well in predicting customer churn in the telecom industry.
**I also exported the trained Machine Learning models so it can be reused for future preductions on new data or even be applied to another problem without retraining the model from scratch.**

## Usage
To replicate and extend this project, follow these steps:
1. Clone the repository:
`git clone` https://github.com/Abdulraqib20/telecom-churn-prediction.git
2. Install the required dependencies:
`pip install -r requirements.txt`
 
 ## Conclusion
Customer churn prediction is a critical task for businesses in the telecom industry. By accurately identifying customers at risk of churning, companies can implement targeted retention strategies to reduce customer attrition and improve customer satisfaction.

This project demonstrates the application of machine learning techniques, specifically XGBoost, for customer churn prediction. The optimized model achieved promising results, providing insights into customer behavior and facilitating data-driven decision-making.
