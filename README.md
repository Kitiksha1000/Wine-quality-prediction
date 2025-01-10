# Wine Quality Analysis and Prediction

## Description:
This project focuses on predicting wine quality based on a dataset of chemical properties and sensory attributes. The analysis includes extensive exploratory data analysis (EDA), feature engineering, and model evaluation to develop a reliable prediction system.

## Features and Data Engineering:

1. Exploratory Data Analysis (EDA): Visualized data distributions and relationships using histograms, scatter plots, and heatmaps to identify patterns and trends in wine quality.
* Wine quality scores range from 3 to 8, with most wines rated as average quality (5 or 6).
* Features exhibit varying scales and distributions.
* Some features are tail-heavy (e.g., residual sugar, free sulfur dioxide).
* Others show multimodal distributions (e.g., volatile acidity, citric acid).
2. Stratified Sampling: Ensured balanced representation across wine quality categories during model training and testing.
  
3. Preprocessing Pipeline:
* Applied missing value imputation using SimpleImputer.
* Standardized features with StandardScaler for consistent input scales.
4. Feature Selection and Creation: Evaluated feature importance for improved predictive accuracy.
  
## Model Building:
Baseline Models: Evaluated multiple regression models using cross-validation:
* Linear Regression:- Shows better precision compared to DecisionTree but struggles with accurately predicting wines of poor and exceptional quality.
* Decision Tree Regressor:- Exhibits overfitting, reducing generalizability to unseen data.
* Random Forest Regressor:- Outperforms LinearRegression and DecisionTree in overall performance.

## Hyperparameter Tuning:
1. Fine-tuned the Random Forest Regressor using GridSearchCV.
2. Achieved optimal parameters, maximizing model performance.

## Performance Metrics:
Final model (Random Forest Regressor) performance:
1. Mean Squared Error (MSE): 0.35
2. Validated results with a 95% confidence interval to ensure reliability.
