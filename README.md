# Unsupervised-Learning-with-the-Iris-Dataset
## Objective
To understand unsupervised learning by applying clustering to the Iris dataset 
and discovering natural groupings without using labels or evaluation metrics.

## Dataset

The Iris dataset contains 150 samples of iris flowers, each described by:

- sepal length (cm)

- sepal width (cm)

- petal length (cm)

- petal width (cm)

## Workflow

### 1. Load the Iris Dataset

The dataset was loaded directly using Python’s built-in dataset library (no CSV file). This provides clean, ready-to-use numerical features.

### 2. Visual Exploration

Before modeling, scatter plots were created to explore relationships between features.
This step helped reveal patterns, separations, and overlapping regions in the dataset.

Examples examined:

petal length vs petal width

sepal length vs sepal width

### 3. Feature Scaling

Scaling was applied using StandardScaler to ensure all features contribute equally to the clustering process. This step is important because K-Means is distance-based and is affected by differences in feature ranges.

### 4. Elbow Method for Choosing k

The elbow method was used to determine the optimal number of clusters. The “elbow point” indicated that 3 clusters was the most suitable choice for this dataset.

### 5. K-Means Clustering

Using the chosen value of k = 3, K-Means was applied to group the samples into clusters based on similarity in their measurements.

### 6. Scatter Plot Visualization

Cluster results were visualized using a scatter plot based on petal length and petal width. Each cluster was plotted in a different color, and the cluster centroids were highlighted to show the center of each group.

## Notebook

The full implementation, including code, and charts is available in the uploaded .ipynb file.

# Questions:

### 1. Why does unsupervised learning not require labeled data?
Because unsupervised learning aims to discover patterns or structure within the data itself—not to predict a known output. Since there is no target variable to learn from, labels are unnecessary.

### 2. Which pair of features seems to show natural groupings?
Petal length and petal width

### 3. Why is feature scaling important when using K-Means?
K-Means uses distance calculations (usually Euclidean distance).
If features are on different scales, the larger-scaled features will dominate the distance and distort the clusters. Scaling ensures each feature contributes fairly.

### 4. What does a cluster centroid represent in simple terms?
A cluster centroid is the center point of a group of similar data points.

### 5. Do the clusters appear clearly separated? Explain your observation.
Yes. Appart from two which are elongated and slightly overlap

### 6. Why is the elbow point a good choice for the number of clusters?
The elbow point is where adding more clusters no longer reduces the within-cluster distortion significantly. It represents a balance between too few clusters (underfitting) and too many clusters (overfitting). The elbow gives a natural and efficient number of clusters.

# Interpretation & Reflection

### 1. What patterns did the clustering algorithm discover?
The algorithm successfully identified 3 clusters corresponding to distinct groupings 
in the data. However, K-Means struggled with non-spherical and overlapping clusters, 
particularly the elongated middle cluster. 

### 2. How many clusters seem reasonable based on the plots?
- 3

### 3. What challenges did you notice when clustering the data?
- Non-spherical cluster shapes
- cluster overlap
