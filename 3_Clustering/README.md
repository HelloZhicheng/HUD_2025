# **Clustering Analysis: Vulnerability and Resilience**



## **Overview**
This folder contains an R script for performing clustering analysis on data related to vulnerability and resilience indices. The analysis uses **K-means**, and **hierarchical clustering**. The script evaluates clustering performance and visualizes the results with several techniques, including the elbow method and silhouette analysis.

## **Features**
1. **Elbow Method**: Identifies the optimal number of clusters.
2. **K-means Clustering**: Groups data into clusters based on centroids.
3. **Hierarchical Clustering**: Groups data hierarchically.
4. **Silhouette Analysis**: Evaluates the quality of clusters for all methods.
5. **Visualization**: Creates scatter plots to show clustering results and relationships between variables.

## **Required Libraries**
Install the following R libraries before running the script:
install.packages(c("readxl", "moments", "scales", "ggplot2", "tidyverse", 
                   "cluster", "factoextra", "dendextend"))

## **Input Data**
The script uses a file named rescaled_index_0610.xlsx as input. This file must contain the following columns:
1. **vul_mean**: Vulnerability index
2. **res_mean**: Resilience index
3. **state**: State information (used to assign cities: Detroit or Cincinnati)

## **Outputs**
1. **cluster_weighted_0617_5cluster_mean.csv**: Cluster assignments for K-means and hierarchical clustering.
2. **Weighted_cluster.pdf**: Visualizations of clustering results.

## **Console Outputs**
1. Average within-cluster standard deviation for K-means and hierarchical clustering.
2. Aggregate cluster means for all methods.
3. Silhouette plots to assess cluster quality.

## **Usage**
1. Place the input file rescaled_index_0610.xlsx in the working directory.
2. Run the script **Clustering.R** in R or RStudio.
3. Review the generated outputs in the working directory.

## **Load and run the script**
source("clustering_analysis.R")

