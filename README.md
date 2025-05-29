#  Calories Burned Prediction Using Machine Learning

**Author**  
[Hanjun Tang]

---

##  Abstract  
This project explores the use of supervised machine learning models to predict calories burned during exercise based on personal physiological attributes. Multiple models were compared, and the neural network showed the highest predictive accuracy (R² = 0.9998). Key findings indicate that heart rate and duration are the most influential predictors. This work supports personalized health monitoring and fitness planning.

---

##  Rationale  
Calorie tracking is critical for managing fitness goals, weight control, and personalized health recommendations. Manual tracking is error-prone and impractical. A data-driven predictive model simplifies this process and provides more accurate, real-time estimates of energy expenditure.

---

##  Research Question  
Can we accurately predict the number of calories burned during an activity using personal attributes (e.g., age, weight, heart rate, duration) with supervised machine learning models?

---

##  Data Sources  
- **Dataset**: [Calories Burnt Prediction Dataset – Kaggle](https://www.kaggle.com/datasets/ruchikakumbhar/calories-burnt-prediction)  
- **Records**: 15,000 samples  
- **Features**: Gender, Age, Height, Weight, Duration, Heart Rate, Body Temperature  
- **Target**: Calories burned

---

## 🛠 Methodology  
1. Data cleaning and feature engineering  
2. Standardization using `StandardScaler`  
3. Model training using:
   - Linear Regression
   - Ridge & Lasso
   - Random Forest
   - XGBoost
   - Neural Network (MLPRegressor)  
4. Hyperparameter tuning with `GridSearchCV`  
5. Evaluation using RMSE and R²  
6. Model explainability via SHAP visualizations

---

##  Results  

| Model              | RMSE (↓) | R² Score (↑) |
|-------------------|-----------|---------------|
| Linear Regression | 11.48     | 0.9670        |
| Ridge Regression  | 11.48     | 0.9670        |
| Lasso Regression  | 11.53     | 0.9669        |
| Random Forest     | 2.64      | 0.9976        |
| XGBoost           | 1.66      | 0.9991        |
| **Neural Network**| **0.79**  | **0.9998**    |

- SHAP analysis confirmed **Duration** and **Heart Rate** as the most important features.

---

##  Next Steps  
- Optimize Neural Network to reduce complexity and runtime.  
- Add polynomial/interaction terms for linear models.  
- Deploy the best model via a web API or mobile fitness tracker app.  
- Investigate anomalies in cross-validation scoring.

---

##  Conclusion  
The project achieved highly accurate predictions of calorie burn using machine learning. The neural network model proved to be the most effective. While the results are promising, model deployment and generalization in real-world environments require further validation and simplification.

---

##  Bibliography  
- Kumbhar, Ruchika. *Calories Burnt Prediction Dataset*. Kaggle, 2021. https://www.kaggle.com/datasets/ruchikakumbhar/calories-burnt-prediction  
- Lundberg, Scott M., and Su-In Lee. “A Unified Approach to Interpreting Model Predictions.” *Advances in Neural Information Processing Systems*, vol. 30, 2017.  
- Pedregosa, Fabian, et al. “Scikit-learn: Machine Learning in Python.” *Journal of Machine Learning Research*, vol. 12, 2011.

---

##  Contact and Further Information  
For questions or collaboration inquiries, please contact:  
 [tanghanjun051026@hotmail.com]  
