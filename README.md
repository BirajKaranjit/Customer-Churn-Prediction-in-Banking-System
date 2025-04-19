# Customer Churn Prediction in Banking-System-Data_Science

This repository presents a machine learning solution for predicting **bank customer churn**. The objective is to accurately identify customers who are likely to discontinue banking services, enabling the institution to implement targeted retention strategies.

## Project Workflow

- Conducted **exploratory data analysis (EDA)** to understand trends, detect outliers, and identify important features.
  ![correlation_heatmap](https://github.com/user-attachments/assets/751573bc-f804-41e8-bc64-87f22ae076a1)

- Performed **data preprocessing**:
  - Handled missing values and outliers using **interquantile range (IQR)** filtering.
  - Applied **one-hot encoding** to convert categorical variables (e.g., *gender*, *country*) into numerical format.
- Evaluated a range of **classification algorithms**:
  - *Logistic Regression*
  - *K-Nearest Neighbors (KNN)*
  - *Decision Tree Classifier*
  - *Random Forest Classifier*
  - *Gradient Boosting Classifier*
  - *Support Vector Machine (SVM)*
  - *Light Gradient Boosting Machine (LightGBMClassifier)*

- Used **10-fold cross-validation** to compare model performances.
- Tuned hyperparameters with `GridSearchCV`, including:
  - *Number of Estimators*
  - *Learning Rate*
  - *Maximum Tree Depth*

## 🏆 Best Model: **LightGBMClassifier**

The best performing model was the **Light Gradient Boosting Machine (LightGBMClassifier)**, tuned using grid search with the following hyperparameters:

- **Learning Rate:** `0.05`  
- **Max Depth:** `5`  
- **Number of Estimators:** `100`

### 🔢 Evaluation Metrics:

- **Accuracy:** `0.8675`  
- **Precision:** `0.7520`  
- **Recall:** `0.4860`  
- **F1 Score:** `0.5904`  
- **ROC-AUC Score:** `0.8731`

## 📊 Model Comparison

### Gradient Boosting Classifier
- **Accuracy:** `0.8640`  
- **Precision:** `0.7530`  
- **Recall:** `0.4711`  
- **F1 Score:** `0.5775`  
- **ROC-AUC:** `0.8698`

### Random Forest Classifier
- **Accuracy:** `0.8605`  
- **Precision:** `0.7938`  
- **Recall:** `0.3919`  
- **F1 Score:** `0.5247`  
- **ROC-AUC:** `0.8685`

