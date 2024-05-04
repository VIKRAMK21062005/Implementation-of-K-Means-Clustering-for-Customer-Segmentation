# Implementation-of-K-Means-Clustering-for-Customer-Segmentation

## AIM:
To write a program to implement the K Means Clustering for Customer Segmentation.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Jupyter notebook

## Algorithm
1.Import dataset and print head,info of the dataset

2.check for null values

3.Import kmeans and fit it to the dataset

4.Plot the graph using elbow method

5.Print the predicted array

6.Plot the customer segments 

## Program:
```
/*
Program to implement the K Means Clustering for Customer Segmentation.
Developed by: VIKRAM K
RegisterNumber:  212222040180
*/
```

```/*
import pandas as pd
import matplotlib.pyplot as plt
data = pd.read_csv("Mall_Customers.csv")
data.head()

data.info()

data.isnull().sum()

from sklearn.cluster import KMeans
wcss = []

for i in range(1,11):
  kmeans = KMeans(n_clusters = i, init = "k-means++")
  kmeans.fit(data.iloc[:, 3:])
  wcss.append(kmeans.inertia_)
  
plt.plot(range(1, 11), wcss)
plt.xlabel("No. of Clusters")
plt.ylabel("wcss")
plt.title("Elbow Method")

km = KMeans(n_clusters = 5)
km.fit(data.iloc[:, 3:])

y_pred = km.predict(data.iloc[:, 3:])
y_pred

data["cluster"] = y_pred
df0 = data[data["cluster"] == 0]
df1 = data[data["cluster"] == 1]
df2 = data[data["cluster"] == 2]
df3 = data[data["cluster"] == 3]
df4 = data[data["cluster"] == 4]

plt.scatter(df0["Annual Income (k$)"], df0["Spending Score (1-100)"], c = "red", label = "cluster0")
plt.scatter(df1["Annual Income (k$)"], df1["Spending Score (1-100)"], c = "black", label = "cluster1")
plt.scatter(df2["Annual Income (k$)"], df2["Spending Score (1-100)"], c = "blue", label = "cluster2")
plt.scatter(df3["Annual Income (k$)"], df3["Spending Score (1-100)"], c = "green", label = "cluster3")
plt.scatter(df4["Annual Income (k$)"], df4["Spending Score (1-100)"], c = "magenta", label = "cluster4")

plt.legend()

plt.title("Customer Segments")

*/
```

## Output:

## DATA TABLE:

![image](https://github.com/VIKRAMK21062005/Implementation-of-K-Means-Clustering-for-Customer-Segmentation/assets/120624033/55d18106-ef33-4cef-8510-9c374c737f91)

## DATA INFO:

![image](https://github.com/VIKRAMK21062005/Implementation-of-K-Means-Clustering-for-Customer-Segmentation/assets/120624033/cb854d51-b8b7-4cde-b1ca-73540c6bfab7)

## NULL VALUES:

![image](https://github.com/VIKRAMK21062005/Implementation-of-K-Means-Clustering-for-Customer-Segmentation/assets/120624033/a2617441-875f-4775-9e53-4e03cdc863bc)

## ELBOW GRAPH:

 ![image](https://github.com/VIKRAMK21062005/Implementation-of-K-Means-Clustering-for-Customer-Segmentation/assets/120624033/22d712c2-057e-4c92-8be6-6723d9c21c7e)

## CLUSTER FORMATION:

![image](https://github.com/VIKRAMK21062005/Implementation-of-K-Means-Clustering-for-Customer-Segmentation/assets/120624033/66a464b7-79e7-460f-be6d-d71fc727ebd5)

## PREDICICTED VALUE:

 ![image](https://github.com/VIKRAMK21062005/Implementation-of-K-Means-Clustering-for-Customer-Segmentation/assets/120624033/b5b71cf3-5596-4dec-961e-817c265e97e2)

## FINAL GRAPH(D/O):

![image](https://github.com/VIKRAMK21062005/Implementation-of-K-Means-Clustering-for-Customer-Segmentation/assets/120624033/b747264e-f7b0-49f0-9a8c-d949451db886)

## Result:
Thus the program to implement the K Means Clustering for Customer Segmentation is written and verified using python programming.
