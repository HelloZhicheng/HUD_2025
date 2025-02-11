# **PCA Analysis**

## **Overview**
This folder contains code and resources for conducting Principal Component Analysis (PCA) to analyze and interpret **exposure**, **sensitivity**, **mitigation**, **preparedness**, **response**, and **recovery** across multiple dimensions such as infrastructure, social, economic, environmental, and health variables. The analysis is aimed at identifying key factors contributing to variability and generating weighted and unweighted indices for comparative analysis. It includes tools for preprocessing, factor analysis, KMO and Bartlett tests, PCA visualization, and correlation analysis.

## **Features of the Analysis**
1. **Data Preprocessing**: 
   - Reads and processes data from multiple Excel sheets (e.g., `Infrastructure_variable`, `Social_variable`).
   - Adjusts the direction of variables (e.g., reversing the sign for specific indicators to ensure consistency).
   - Combines all variables into a unified dataset for PCA.

2. **Assumption Tests**:
   - **Kaiser-Meyer-Olkin (KMO) Test**: Ensures sampling adequacy for PCA.
   - **Bartlett's Test of Sphericity**: Validates the factorability of the dataset.

3. **Principal Component Analysis**:
   - Standardizes the data before PCA.
   - Extracts principal components and visualizes their contributions using scree plots and variable loading plots.
   - Computes eigenvalues and variance explained for each component.

4. **Weighted and Unweighted Indices**:
   - Generates unweighted scores by averaging principal component scores.
   - Creates weighted scores by combining component scores with their proportional variance contributions.

5. **Factor Rotation**:
   - Applies varimax rotation to interpret factor loadings more effectively.
   - Exports rotated component matrices and their explained variances.

6. **Correlation Analysis**:
   - Produces a correlation matrix of variables and visualizes it using correlation plots.

## **Required Libraries**
Install the following R libraries before running the script: `readxl`, `tidyverse`, `devtools`, `ggbiplot`, `factoextra`, `FactorAssumptions`, `EFAtools`, `pracma`, `corrplot`

## **Usage**
1. **Dataset**: Ensure the input Excel file (e.g., `Final_Sensitivity.xlsx`) is available in the specified path. The file should include sheets with variables related to infrastructure, social, economic, environmental, and health dimensions.

2. **Run the Script**:
   - Load the script and execute it in R.
   - Perform KMO and Bartlett tests to check dataset suitability for PCA.
   - Conduct PCA to extract principal components and visualize results.
   - Generate weighted and unweighted indices for each observation.
   - Save the results (e.g., scores, rotated loadings, variance explained) as CSV files.

3. **Outputs**:
   - PCA results: Scree plots, variable contributions, and component scores.
   - Indices: Weighted and unweighted scores with ranks.
   - Factor matrices: Rotated and unrotated loadings for components.
   - Correlation matrix: Visualized as a plot.

4. **Interpretation**:
   - Use scree plots and loading plots to identify key components and variables.
   - Analyze weighted and unweighted scores for sensitivity comparisons across dimensions.

## **Contributors**
If you have questions or suggestions for improving the analysis or script, feel free to open an issue or submit a pull request.
