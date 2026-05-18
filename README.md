# Implementation-of-K-Means-Clustering-for-Customer-Segmentation

## AIM:
To write a program to implement the K Means Clustering for Customer Segmentation.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Jupyter notebook

## Algorithm

1. Read the customer dataset and select Annual Income and Spending Score as input features.
2. Initialize the K-Means model with 5 clusters and fit the model to the dataset.
3. Predict the cluster for each customer and group similar customers together.
4. Plot the clustered customers and display the cluster centroids using a scatter graph.

## Program:
```
/*
Program to implement the K Means Clustering for Customer Segmentation.

# Simple K-Means Clustering Program for Customer Segmentation

import pandas as pd
import matplotlib.pyplot as plt
from sklearn.cluster import KMeans

data = pd.read_csv("Mall_Customer.csv")

X = data.iloc[:, [3, 4]].values

kmeans = KMeans(n_clusters=5, random_state=0)

y_kmeans = kmeans.fit_predict(X)

plt.scatter(X[:, 0], X[:, 1], c=y_kmeans, s=50)

# Plot centroids
plt.scatter(kmeans.cluster_centers_[:, 0],
            kmeans.cluster_centers_[:, 1],
            s=200,
            marker='X')

# Labels
plt.xlabel("Annual Income")
plt.ylabel("Spending Score")
plt.title("Customer Segmentation using K-Means")

plt.show()

Developed by: MAHAMMED AMEER F
RegisterNumber: 212225040248
*/
```

## Output:
<img width="1064" height="641" alt="WhatsApp Image 2026-05-18 at 1 06 21 PM" src="https://github.com/user-attachments/assets/61a8c0d6-e8f9-4768-b090-08e7b9830e6b" />

## Result:
Thus the program to implement the K Means Clustering for Customer Segmentation is written and verified using python programming.
