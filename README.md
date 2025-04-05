🌦 Weather Prediction with Random Forest

📌 Project Overview

This project aims to build a predictive model for forecasting temperature values using weather data. The model leverages various machine learning algorithms.
After extensive hyperparameter tuning, the Random Forest Regressor achieved the best performance.

 📁 Dataset
 Source:Dataset (`Bias_correction_ucl.csv`) 


⚙️ Project Workflow
1. Data Preprocessing:
   - Handling missing values using different techniques (Mode, Median, KNN Imputation).
   - Dropping irrelevant or highly missing columns.
   - Scaling numerical features where necessary.

2. Model Building:
   - Baseline Models: Linear Regression, Decision Tree Regressor
   - Advanced Models: Random Forest Regressor, Gradient Boosting, XGBoost

3. Hyperparameter Tuning:
   - Using `GridSearchCV` to find the best parameters for the Random Forest Regressor.

4. Model Evaluation:
   - Performance Metrics: MSE, R² Score
   - Best Model Achieved: Random Forest Regressor with R² Score of 0.914

5. Deployment (Future Work):
   - Deploying the model using Flask.

 📈 Results
- The best performing model was the **Random Forest Regressor with the following hyperparameters:
  - `max_depth`: None
  - `max_features`: 'sqrt'
  - `min_samples_leaf`: 1
  - `min_samples_split`: 2
  - `n_estimators`: 300

- R² Score: 0.914
- Mean Squared Error (MSE): 0.696

 📂 File Structure
```
├── Bias_correction_ucl.csv           # Original dataset
├── optimized_random_forest_model.pkl # Saved model file
└── bias2.ipynb.ipynb               # Jupyter Notebook with all steps
```



📌 Future Improvements
- Implement model deployment using Flask.
- Test additional machine learning models (e.g., LightGBM, CatBoost).
- Implement feature engineering for improved predictions.

 📄 License
This project is licensed under the MIT License.


