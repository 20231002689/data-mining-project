# Non-Technical Summary: Calories Burned Prediction Project

## Problem Statement
This project aims to predict calories burned using personal attributes such as gender, age, height, weight, exercise duration, heart rate, and body temperature.<br>
The prediction model can be applied in health monitoring and fitness planning, helping users better manage their daily exercise and diet.

## Dataset
Data sources：https://www.kaggle.com/datasets/ruchikakumbhar/calories-burnt-prediction  
Data structure:Contains 15,000 records, 7 features: Gender, Age, Height, Weight, Duration, Heart_Rate, Body_Temp  
Target variable: Calories (calories burned)

## Key Findings
- Several machine learning models were used, including Linear Regression, Random Forest, XGBoost, and Neural Network.<br>
- The Neural Network performed the best, with a prediction accuracy (R²) of 99.98% and an average error (RMSE) of only 0.79 calories.<br>
- Random Forest came in second, with an R² of 99.83% and an RMSE of 2.62 calories.<br>
- Exercise duration and heart rate were identified as the most important factors affecting calorie burn.

## Model Performance
Below is an overview of the main models' performance:
| Model            | Average Error (RMSE) | Accuracy (R²) |
|------------------|---------------------|---------------|
| Linear Regression | 11.48               | 0.9670        |
| Ridge Regression  | 11.48               | 0.9670        |
| Lasso Regression  | 11.53               | 0.9669        |
| Random Forest     | 2.64                | 0.9976        |
| XGBoost           | 1.66                | 0.9991        |
| Neural Network    | 0.79                | 0.9998        |

- The Neural Network excelled in predicting calories burned, making it ideal for high-precision needs.<br>
- Linear(Ridge,Lasso) Regression had a higher error due to its inability to capture non-linear patterns in the data.

## Potential Improvements
- Add polynomial features or interaction terms to improve the Linear Regression model's predictions.<br>
- Optimize the Neural Network's structure to reduce computational cost and improve practicality.<br>
- Investigate and fix anomalies in cross-validation results (e.g., unusually small MSE values) to ensure reliability.

## Project Files
- `calories.csv`: The project dataset, containing 15,000 records and 7 features.
- `calories_prediction_project.ipynb`: Technical report detailing data preprocessing, model training, and evaluation steps.
- `figures/`: Contains data visualizations (e.g., histograms, correlation heatmaps, and prediction plots).
- `requirements.txt`: List of required libraries.
- This `README.md`: Non-technical summary.
