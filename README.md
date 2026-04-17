# Customer Segmentation — Paragon Corp Use Case

Segmenting mall customers into distinct groups using K-Means Clustering

## Overview
A machine learning clustering project that segments customers based on 
their annual income and spending behavior. This project simulates a 
real-world use case for companies like Paragon Corp to identify target 
customer groups and optimize their marketing strategy.

## Problem Statement
Understanding customer behavior is critical for any retail or FMCG company. 
Without proper segmentation, marketing budgets are wasted targeting the wrong 
audience. This project uses unsupervised machine learning to group customers 
into meaningful segments, enabling more focused and effective marketing decisions.

## Dataset
- Source: [Customer Clustering Dataset](https://www.kaggle.com/datasets/dev0914sharma/customer-clustering)
- Features used: Annual Income (k$), Spending Score (1-100)
- Total records: 200 customers

## Tools & Technologies
- Python
- Google Colab
- Pandas, NumPy, Scikit-learn, Matplotlib, Seaborn

## Methodology
1. Exploratory Data Analysis (EDA)
   - Distribution analysis of Age, Annual Income, Spending Score
   - Scatter plot to visually identify potential clusters
2. Optimal Cluster Selection
   - Elbow Method — identified drop point at k=5
   - Silhouette Score — confirmed k=5 as optimal (score: 0.5547)
3. Model Implementation — K-Means Clustering (k=5)
4. Cluster Interpretation & Business Insight

## Results

|      Metric      | Score  |
|------------------|--------|
| Inertia          | 65.57  |
| Silhouette Score | 0.5547 |

## Customer Segments Identified

| Cluster |    Segment Name    |         Characteristics          |
|---------|--------------------|----------------------------------|
|    1    | Careful Spenders   | Low income, low spending         |
|    2    | Impulsive Buyers   | Low income, high spending        |
|    3    | Conservative Rich  | High income, low spending        |
|    4    | Target Customer    | High income, high spending       |
|    5    | Standard Customers | Average income, average spending |

## Business Insight
- **Target Customer** segment is the highest priority for premium product campaigns
- **Impulsive Buyers** respond well to promotions and limited time offers
- **Conservative Rich** need value-based marketing to convert their spending potential
- **Standard Customers** represent the largest group and are ideal for mid-range products

## How to Run
1. Download the dataset from the Kaggle link above
2. Open `Customers_Segmentation.ipynb` in Google Colab
3. Update the file path to match where you saved the dataset
4. Run all cells
