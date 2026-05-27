# SmartCart — Customer Segmentation System

A machine learning project that segments retail customers into distinct behavioral groups using unsupervised learning techniques. Built on a real-world dataset of 2,240 customers, the pipeline covers data preprocessing, feature engineering, dimensionality reduction, and clustering.

---

## Overview

| Detail | Info |
|---|---|
| Dataset | 2,240 customer records |
| Task | Unsupervised clustering |
| Models | K-Means, Agglomerative Clustering |
| Dimensionality Reduction | PCA (3 components) |
| Optimal Clusters | k = 4 |

---

## What it does

- Cleans raw customer data handles missing income values, removes outliers, and standardizes education and marital status labels
- Engineers meaningful features such as total spending, customer tenure, age, and household size
- Encodes categorical variables and scales all features before modeling
- Reduces dimensionality using PCA and determines the optimal number of clusters via the Elbow Method and Silhouette Score
- Compares K-Means and Agglomerative Clustering and profiles each segment by income, spending, and purchase behavior

---

## Tech Stack

`Python` `Pandas` `Scikit-learn` `Matplotlib` `Seaborn` `Kneed` `Jupyter Notebook`

---

## How to Run

```bash
pip install pandas scikit-learn matplotlib seaborn kneed
jupyter notebook smartcart.ipynb
```

---

## Results

The model identifies **4 distinct customer segments** differentiated by income level, total spending across product categories, purchase recency, and household composition. Segment profiles are summarized using mean-aggregated feature values, making the output directly usable for marketing and targeting decisions.

