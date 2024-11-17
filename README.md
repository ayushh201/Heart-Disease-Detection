# Heart Disease Detection Project

## Overview  
This project aims to predict the presence of heart disease in patients based on clinical data. It includes **Exploratory Data Analysis (EDA)** and the development of machine learning models for accurate predictions. By analyzing key features like age, chest pain type, and cholesterol levels, the project highlights patterns and trends associated with heart disease risks.


## Dataset Description  
The dataset includes clinical features and diagnostic results for heart disease detection. Here's a breakdown of the features:

| **Feature**      | **Description**                                                                 | **Importance**                                                                                                     |
|-------------------|---------------------------------------------------------------------------------|---------------------------------------------------------------------------------------------------------------------|
| `age`            | Age of the patient in years                                                     | Older individuals are at higher risk of heart disease.                                                             |
| `sex`            | Gender of the patient (1 = male, 0 = female)                                    | Males are generally at a higher risk of heart disease.                                                             |
| `cp`             | Chest pain type (0-3)                                                           | Indicates the likelihood and nature of heart problems, with asymptomatic pain suggesting severe disease.            |
| `trestbps`       | Resting blood pressure (mm Hg)                                                  | High values (>130-140 mm Hg) are a major risk factor.                                                              |
| `chol`           | Serum cholesterol (mg/dl)                                                      | High cholesterol levels (>200 mg/dl) increase risk.                                                                |
| `fbs`            | Fasting blood sugar >120 mg/dl (1 = true, 0 = false)                            | Indicates diabetes, a risk factor for heart disease.                                                               |
| `restecg`        | Resting electrocardiographic results (0-2)                                      | Abnormal readings indicate potential heart conditions.                                                             |
| `thalach`        | Maximum heart rate achieved                                                    | Lower heart rates during exercise can indicate reduced heart fitness.                                              |
| `exang`          | Exercise-induced angina (1 = yes, 0 = no)                                       | Strongly indicates coronary artery disease.                                                                        |
| `oldpeak`        | ST depression induced by exercise relative to rest                              | Signals ischemia, a condition of reduced blood flow to the heart.                                                 |
| `slope`          | Slope of peak exercise ST segment (0-2)                                         | Downsloping segments often indicate poor heart health.                                                             |
| `ca`             | Number of major vessels (0-3) colored by fluoroscopy                           | A higher count suggests better heart health.                                                                       |
| `thal`           | Thallium stress test result (1, 3, 6, 7)                                        | Abnormal results suggest fixed or reversible defects indicating reduced blood flow.                                |
| `target`         | Presence of heart disease (1 = yes, 0 = no)                                     | The variable to predict.                                                                                           |


## Project Workflow  

### 1. Understanding the Problem Statement  
- Predict whether a patient has heart disease based on clinical data.  

### 2. Data Collection  
Link - https://www.kaggle.com/datasets/johnsmith88/heart-disease-dataset?resource=download

### 3. Data Preprocessing  
- **Missing Values:** Imputed or handled appropriately.  
- **Categorical Variables:** Encoded using one-hot or label encoding (e.g., chest pain type, thal).  
- **Scaling:** Continuous variables like age, cholesterol, and blood pressure scaled using `StandardScaler`.  

### 4. Exploratory Data Analysis (EDA)  
- **Correlation Heatmaps:** Identify relationships between features.  
- **Distribution Plots:** Visualize the spread and patterns of key features.  

### 5. Modeling and Implementation  
Three models were trained for heart disease prediction:  
1. **Logistic Regression**  
2. **K-Nearest Neighbors (KNN)**  
3. **Random Forest Classifier**  

#### Hyperparameter Tuning  
- **GridSearchCV:** Applied to optimize model parameters.  


## Evaluation Metrics  

- **Confusion Matrix:** Visualize true/false positives and negatives.  
- **Precision:** Accuracy of positive predictions.  
- **Recall:** Ability to identify actual positives.  
- **F1 Score:** Balances precision and recall.  
- **ROC Curve:** Assesses trade-off between sensitivity and specificity.  


## Results  
- **Best Model:** Random Forest Classifier achieved the highest performance with optimized parameters. (Accuracy - 0.9853658536585366)
- **Key Observations:** Age, chest pain type, and maximum heart rate were highly influential in predictions.  


## Future Enhancements  
- Implement additional models like Gradient Boosting.  
- Include more features like family medical history.  
- Develop a web-based interface for predictions.


## References  
- Scikit-learn Documentation: https://scikit-learn.org/  
- Dataset Source: [UCI Machine Learning Repository](https://archive.ics.uci.edu/ml/datasets/Heart+Disease)  


Contributions are welcome! 😊  
Feel free to fork the repository and submit pull requests.
