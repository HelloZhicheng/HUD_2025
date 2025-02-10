# **Random Forest Models**

## **Overview**
This folder contains code and resources for modeling **exposure**, **sensitivity**, **vulnerability**, **mitigation**, **preparedness**, **response**, **recovery**, **resilience** in areas characterized by **HH** (High Vulnerability and High Resilience) and **HL** (High Vulnerability and Low Resilience). The model uses a combination of feature selection techniques, Random Forest Regressors, and interpretability tools like SHAP to identify critical factors influencing exposure, sensitivity, vulnerability, mitigation, preparedness, response, recovery, and resilience.

## **Features of the Model**
1. **Data Handling and Preprocessing**: Reads and processes data from a CSV file (e.g., `1_exposure_HH.csv`).
Removes unnecessary columns to prepare the dataset for training and testing.
2. **Random Forest Regression**: Uses `RandomForestRegressor` with hyperparameter tuning via `GridSearchCV` to optimize performance; Includes cross-validation and out-of-bag scoring for robust performance evaluation.
3. **Feature Selection**: Sequential Feature Selector (`SequentialFeatureSelector`) is used to identify important features; SHAP values are used for interpretability.
4. **Model Evaluation Metrics**: Cross-validated R² scores (`R2_CV`); Out-of-bag R² scores (`R2_oob`); Root Mean Squared Error (RMSE); Mean Absolute Error (MAE); Standard R² scores.

## **Required Libraries**
Install the following R libraries before running the script: `numpy`, `pandas`, `matplotlib"` `seaborn`, `statsmodels`, `sklearn`, `eli5`, `shap`.

## **Usage**
1. **Dataset**: Ensure the input dataset (e.g., 1_exposure_HH.csv) is present in the same directory. The dataset should contain target variable and predictor variables.
2. **Run the Code**: Execute the script to train the model, tune hyperparameters, evaluate performance, and interpret the results. The code includes hyperparameter tuning with GridSearchCV, feature selection, and performance metrics.
3. **Outputs**: Performance metrics (R², RMSE, MAE), SHAP summary plots.
4. **Interpretation**: Use SHAP plots to interpret how features influence predictions.

## **Contributors**
If you have questions or suggestions for improving the code, feel free to open an issue or submit a pull request.
