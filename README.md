Project Summary
Title : Predicting Age-Related Disease Risk Using Machine Learning

Objective :
This study aims to predict the risk of age-related diseases (e.g., cardiovascular disease) using machine learning models. By leveraging demographic, laboratory, examination, diet, medication, and questionnaire data, the project identifies key predictors of disease risk and provides actionable insights for personalized healthcare interventions.

Methodology :

Data Integration :
Merged multiple datasets (demographic.csv, labs.csv, examination.csv, diet.csv, medications.csv, questionnaire.csv) using a common identifier (SEQN).
Target Variable :
Defined a binary target variable indicating the risk of cardiovascular disease based on thresholds for BMI (>30) and total cholesterol (>240 mg/dL).
Preprocessing :
Handled missing values using mean imputation for numeric features and most frequent value imputation for categorical features.
Scaled numeric features and one-hot encoded categorical features.
Removed features with all missing values to ensure consistency.
Model Training :
Trained three machine learning models:
Random Forest
Gradient Boosting
Neural Network
Evaluation Metrics :
Evaluated model performance using accuracy, precision, recall, F1 score, and ROC AUC.
Feature Importance :
Extracted and visualized feature importance for the best-performing model to identify key predictors of disease risk.
Results
Model Performance
The following table summarizes the performance of the three machine learning models trained to predict the risk of age-related diseases:
Results
Model Performance
Gradient Boosting emerged as the best-performing model with:
Accuracy : 98.77%
Precision : 98.40%
Recall : 98.40%
F1 Score : 98.40%
ROC AUC : 99.89%
Random Forest performed well but slightly trailed behind Gradient Boosting:
Accuracy : 97.73%
Precision : 98.42%
Recall : 95.60%
F1 Score : 96.99%
ROC AUC : 99.77%
Neural Network achieved lower scores compared to the tree-based models:
Accuracy : 96.68%
Precision : 96.16%
Recall : 95.13%
F1 Score : 95.64%
ROC AUC : 99.22%
The Gradient Boosting model performed the best across all metrics.
Top Predictors :
Weight (BMXWT) : 30.86%
Arm Circumference (BMXARMC) : 26.37%
Triglycerides (LBDTCSI) : 15.17%
Waist Circumference (BMXWAIST) : 10.47%
Height (BMXHT) : 5.61%
Key Insights :

Anthropometric measurements (e.g., weight, waist circumference) and biomarkers (e.g., triglycerides) are the most important predictors of cardiovascular disease risk.
Lifestyle factors (e.g., questionnaire responses) also play a significant role, albeit to a lesser extent.
The Gradient Boosting model is highly effective for predicting disease risk and should be used for deployment.
Applications :
This predictive model can be integrated into healthcare systems to:

Identify patients at high risk of age-related diseases.
Enable early intervention through personalized recommendations (e.g., weight management, dietary changes).
Support proactive and preventive healthcare strategies.
Repository Contents :

Code : Python scripts for data preprocessing, model training, evaluation, and visualization.
Datasets : Instructions for loading and merging datasets.
Results : Model performance metrics and feature importance analysis.
Visualization : Bar plots of top predictors for interpretability.
Future Work :

Extend the model to predict risks for other age-related diseases (e.g., diabetes, hypertension).
Incorporate additional features (e.g., genetic data, epigenetic markers).
Optimize hyperparameters for improved performance.
