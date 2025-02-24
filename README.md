# Global Superstore Data Analysis and Customer Segmentation

This project analyzes the Kaggle Global Superstore dataset, a comprehensive collection of sales and order data from a global superstore. The project performs exploratory data analysis (EDA), calculates key performance indicators (KPIs), and implements customer segmentation using K-Means clustering. The goal is to provide strategic insights into business performance and identify opportunities for growth and profitability.

## Project Overview

The analysis focuses on the following key areas:

*   **Data Exploration:** Understanding the dataset's structure, identifying data types, and checking for missing values.
*   **KPI Calculation:** Defining and calculating key metrics, including:
    *   **Average Order Value (AOV)**
    *   **Order Frequency**
    *   **Customer Lifetime Value (CLV)**
    *   **Average Profit**
*   **Customer Segmentation:** Using K-Means clustering to group customers based on CLV and average profit.
*   **Cluster Analysis:**  Analyzing the characteristics of each customer segment (e.g., product category preferences, segment distribution, regional distribution) and providing tailored recommendations.

## Repository Structure

*   **`README.md`**: This file.
*   **`notebooks/`**: Contains the Jupyter Notebook (`Global_Super_Data.ipynb`) with the complete analysis.
*   **`data/`**: Contains the `superstore.csv` dataset.  *It is assumed that the user has downloaded the dataset and placed it in this directory.*

## Data

The dataset used in this project is the "Global Superstore" dataset from Kaggle. You can find the dataset here: [Insert Kaggle Dataset Link Here]. Download the dataset and save it as `superstore.csv` in the `data/` directory. The original dataset (.txt file) has be transform with R language to CSV file.

## Key Findings and Recommendations

The analysis identifies four distinct customer segments based on CLV and average profit.  Detailed descriptions of each segment, along with tailored recommendations for marketing and sales strategies, are provided within the Jupyter Notebook (`global_superstore_analysis.ipynb`). Key areas of focus include:

*   **Identifying and addressing a low-value, unprofitable customer segment (Cluster 0).**
*   **Developing strategies to increase the value of low-value, low-profitability customers (Cluster 1).**
*   **Leveraging the high CLV of moderately profitable customers (Cluster 2) through upselling and loyalty programs.**
*   **Retaining and maximizing the value of high-value, highly profitable customers (Cluster 3).**

The notebook provides detailed visualizations (cluster plots, distribution charts) and statistical summaries to support these findings.

## Methodology

The project follows these key steps:

1.  **Data Loading and Preprocessing:**  The CSV dataset is loaded, basic data cleaning is performed (removing unnecessary columns), and missing values are checked.
2.  **KPI Calculation:**  Key metrics (AOV, Order Frequency, CLV, Average Profit) are calculated using vectorized Pandas operations.
3.  **Outlier Handling:** Winsorization is used to mitigate the impact of extreme values on the clustering process.
4.  **Data Scaling:**  `StandardScaler` is used to scale the data before clustering.
5.  **Clustering:**  K-Means clustering is performed, with the optimal number of clusters (k=4) determined using the elbow method and silhouette score analysis.
6.  **Cluster Analysis:**  The characteristics of each cluster are examined, including the distribution of product categories, customer segments, and regions.
7.  **Recommendations:** Data-driven recommendations are provided for each customer segment to optimize marketing and sales strategies.

## References

*   Kotler, P., & Keller, K. L. (2016). *Marketing Management* (15th ed.). Pearson.
*   Gupta, S., & Lehmann, D. R. (2005). *Managing Customers as Investments: The Strategic Value of Customers in the Long Run*. Wharton School Publishing.
