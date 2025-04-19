# Customer Churn Prediction in Banking-System-Data_Science
Customer Churn Prediction
This repository presents a machine learning-based solution for predicting bank customer churn. The primary objective is to identify customers who are likely to leave the bank (churn), enabling proactive retention strategies. The workflow includes comprehensive Exploratory Data Analysis (EDA), data preprocessing, model training using multiple machine learning algorithms, and rigorous model evaluation.

Workflow Summary:
Conducted detailed EDA to understand feature distributions and correlations.

Performed data cleaning, encoding of categorical variables (via one-hot encoding), and outlier detection.

Trained and evaluated multiple models including:

Logistic Regression

K-Nearest Neighbors (KNN)

Decision Tree Classifier

Random Forest Classifier

Gradient Boosting Classifier

Support Vector Machine

Light Gradient Boosting Machine (LightGBM)

Compared their performance using 5-fold and 10-fold cross-validation strategies.

Carried out hyperparameter tuning using GridSearchCV, optimizing parameters such as:

n_estimators

max_depth

learning_rate (for boosting models)

Best Model: LightGBMClassifier
The Light Gradient Boosting Machine (LightGBMClassifier) outperformed all other models in terms of overall balance between precision and recall. The optimal model configuration after tuning was:

learning_rate = 0.05

max_depth = 5

n_estimators = 100

Evaluation Metrics on Test Set:

Accuracy: 0.8675

Precision: 0.7520

Recall: 0.4860

F1 Score: 0.5904

ROC-AUC: 0.8731

Confusion Matrix:

lua
Copy
Edit
[[1544   63]
 [ 203  192]]
Comparison with Other Models:
Gradient Boosting Classifier:

Accuracy: 0.8640

Precision: 0.7530

Recall: 0.4711

F1 Score: 0.5775

ROC-AUC: 0.8698

Random Forest Classifier:

Accuracy: 0.8605

Precision: 0.7938

Recall: 0.3919

F1 Score: 0.5247

ROC-AUC: 0.8685

Although models like Random Forest and Gradient Boosting showed competitive performance in terms of precision and ROC-AUC, LightGBM offered a better trade-off between precision, recall, and overall generalization.

Future Scope:
Further improvements may be possible by experimenting with ensemble techniques or advanced methods such as stacking and feature selection strategies to enhance recall while preserving precision.
