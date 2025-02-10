# **Multinomial Logistic Regression (MLR) Analysis**

## **Overview**
This folder contains an R script for performing **multinomial logistic regression (MLR)** using the `glmnet` package. The script handles data preprocessing, hyperparameter tuning, model fitting, evaluation, and coefficient uncertainty estimation using bootstrap resampling.

## **Features**
1. **Data Splitting**: Splits data into training (70%) and testing (30%) sets.  
2. **Cross-Validation**: Identifies the optimal value of lambda using ridge regression (`alpha = 0`).  
3. **Model Fitting**: Fits an MLR model using the selected lambda value.  
4. **Predictions and Evaluation**: Generates predictions for the test set and evaluates model accuracy using a confusion matrix.
5. **Coefficient Extraction**: Extracts and interprets model coefficients.  
6. **Deviance Ratio**: Computes the deviance ratio to measure the goodness-of-fit of the model.
7. **Bootstrap Resampling**: Estimates coefficient uncertainty by resampling data 1,000 times and calculating standard errors and p-values for coefficients.  

## **Required Libraries**
Install the following R libraries before running the script: `glmnet`, `dplyr`.

## **Input Data**
1. **Target Variable**: A categorical variable representing classes (e.g., Cluster_result)
2. **Predictor Variables**: Numeric columns representing predictors. The script uses the following predictors: exp_mean, sen_mean, m_mean, pre_mean, rec_mean, res_mean

## **Outputs**
The script outputs the model coefficients for each class in the multinomial logistic regression.

## **Usage**
1. Place the input file **Cluster_result.csv** in the working directory.
2. Run the script **Multinomial Logistic Regression.Rmd** in R or RStudio.
3. Examine the outputs in the console to interpret the model performance and coefficients.

## **Load and Run the Script**
source("Multinomial Logistic Regression.Rmd")

## **Contributors**
If you have questions or suggestions for improving the code, feel free to open an issue or submit a pull request.
