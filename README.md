# Unsupervised-Learning-with-the-Iris-Dataset
## Objective
To understand unsupervised learning by applying clustering to the Iris dataset 
and discovering natural groupings without using labels or evaluation metrics.

## Dataset

The Iris dataset has  the following features:
Sepal Length, Sepal Width, Petal Length, Petal Width

# Questions:

## Why does unsupervised learning not require labeled data?
Because unsupervised learning aims to discover patterns or structure within the data itself—not to predict a known output. Since there is no target variable to learn from, labels are unnecessary.

## Which pair of features seems to show natural groupings?
Petal length and petal width

## Why is feature scaling important when using K-Means?
K-Means uses distance calculations (usually Euclidean distance).
If features are on different scales, the larger-scaled features will dominate the distance and distort the clusters. Scaling ensures each feature contributes fairly.

## What does a cluster centroid represent in simple terms?
A cluster centroid is the center point of a group of similar data points.

## Do the clusters appear clearly separated? Explain your observation.
Yes. Appart from two which are elongated and slightly overlap

## Why is the elbow point a good choice for the number of clusters?
The elbow point is where adding more clusters no longer reduces the within-cluster distortion significantly. It represents a balance between too few clusters (underfitting) and too many clusters (overfitting). The elbow gives a natural and efficient number of clusters.

# Interpretation & Reflection

## What patterns did the clustering algorithm discover?
The algorithm successfully identified 3 clusters corresponding to distinct groupings 
in the data. However, K-Means struggled with non-spherical and overlapping clusters, 
particularly the elongated middle cluster. 

## How many clusters seem reasonable based on the plots?
3

## What challenges did you notice when clustering the data?
Non-spherical cluster shapes
cluster overlap
