# **Analysis Workflow for Vulnerability and Resilience**

This repository outlines the step-by-step workflow for analyzing **vulnerability** and **resilience** using social, economic, environmental, infrastructure, and health data. Below is a summary of the five main steps and their relationships.

---

## **1. Data Collection**
This step retrieves and processes social, economic, and health data from the US Census Bureau API for census tracts in Michigan and Ohio (2010–2020). The outputs are annual datasets used for subsequent analyses.

---

## **2. Principal Component Analysis (PCA)**
The collected data is analyzed using PCA to derive metrics for 

**subindexes**:
- **Exposure**
- **Sensitivity**
- **Mitigation**
- **Preparedness**
- **Response**
- **Recovery**

From these subindexes:
- **Vulnerability** is calculated by combining **Exposure** and **Sensitivity**.
- **Resilience** is calculated by combining **Mitigation**, **Preparedness**, **Response**, and **Recovery**.

---

## **3. Clustering Analysis**
Using the **Vulnerability** and **Resilience** indexes from Step 2, clustering analysis is conducted to classify data into distinct groups. This step employs K-means and hierarchical clustering techniques to categorize the data based on levels of vulnerability and resilience.

---

## 4. Multinomial Logistic Regression (MNL)
Multinomial Logistic Regression is performed to explore how the subindexes (**Exposure**, **Sensitivity**, **Mitigation**, **Preparedness**, **Response**, and **Recovery**) influence the vulnerability and resilience categories obtained in Step 3.

---

## 5. Random Forest Analysis
Random Forest models are used to identify the most critical indicators for each subindex (**Exposure**, **Sensitivity**, **Mitigation**, **Preparedness**, **Response**, and **Recovery**). This step helps interpret the factors driving the system's vulnerability and resilience.

---

## Workflow Summary
1. **Data Collection** ➔ Retrieve and preprocess input data.
2. **PCA Analysis** ➔ Calculate subindexes and derive **Vulnerability** and **Resilience**.
3. **Clustering Analysis** ➔ Classify data based on **Vulnerability** and **Resilience** indexes.
4. **Multinomial Logistic Regression** ➔ Analyze subindex influences on classifications.
5. **Random Forest Analysis** ➔ Identify critical indicators influencing subindexes.

---

This workflow provides a comprehensive approach to understanding and interpreting vulnerability and resilience across multiple dimensions.
