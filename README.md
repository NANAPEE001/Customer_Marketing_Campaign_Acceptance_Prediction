# Customer Marketing Campaign Acceptance Prediction

This project focuses on predicting whether a customer will accept a marketing campaign based on their demographic data, purchase behavior, and previous campaign interactions. The dataset was cleaned, preprocessed, and analyzed using several machine learning models, including Random Forest, XGBoost, and logistic regression. The models are evaluated based on their ability to predict customer responses, with performance measured using ROC-AUC.

Data Preprocessing
The dataset included some missing values, especially in the Income column, which were replaced with the median value. Duplicates were identified and removed to ensure the integrity of the data. Categorical variables like Marital_Status and Response were converted into factors for modeling, while the Dt_Customer column was used to extract additional temporal features such as Year and Month. The target variable, Response, was recoded to ensure consistency for model training.

Exploratory Data Analysis (EDA)
The data was explored visually using boxplots and bar charts to examine the relationships between features like Recency, NumWebPurchases, and the target Response. The distribution of the target variable was also analyzed to understand customer response patterns.

Modeling
Various classification models were built, including Random Forest, XGBoost, and logistic regression with both forward and backward feature selection. Additionally, LASSO regression was employed to handle high-dimensional data. Each model was trained and tested using a training-test split of 80-20% to ensure robust evaluation.

Model Evaluation
The performance of each model was evaluated using ROC curves and AUC scores. The models were fine-tuned using cross-validation to optimize hyperparameters. 

SHAP Analysis
SHAP values were calculated for the XGBoost model to explain the importance of each feature in the decision-making process. SHAP dependence plots were used to visualize how key features like NumStorePurchases and Income influence model predictions.
