# Day 12 - Mean Shift Clustering

This project is part of my Machine Learning learning journey, where I implemented 
**Mean Shift Clustering** using Python and Scikit-learn.

## Project Overview

Mean Shift is a **non-parametric unsupervised learning algorithm** used for clustering data 
points based on their density in feature space. Unlike algorithms such as K-Means, Mean Shift
does not require specifying the number of clusters beforehand.

In this project, I created synthetic 3D data points using `make_blobs`, applied the Mean
Shift clustering algorithm, estimated the bandwidth automatically, and visualized both the 
raw data points and the cluster centers.

## What This Project Covers

- Understanding the concept of Mean Shift Clustering
- Generating synthetic 3D sample data
- Estimating bandwidth using `estimate_bandwidth`
- Applying `MeanShift` from Scikit-learn
- Finding cluster centers automatically
- Visualizing clustered data in 3D

## Technologies Used

- Python
- NumPy
- Matplotlib
- Scikit-learn
- Google Colab / Jupyter Notebook

## Libraries Used

```python
import numpy as np
import matplotlib.pyplot as plt
from sklearn.cluster import MeanShift, estimate_bandwidth
from sklearn.datasets import make_blobs
from mpl_toolkits.mplot3d import Axes3D
```

## Workflow

1. Import required libraries
2. Define sample 3D coordinates
3. Generate synthetic data using `make_blobs`
4. Visualize the raw data in a 3D plot
5. Estimate bandwidth automatically
6. Apply Mean Shift clustering
7. Extract cluster centers and labels
8. Count the number of clusters formed
9. Visualize the clustered points and their centers

## Key Concept

Mean Shift works by shifting each data point toward the **nearest high-density region** 
in the dataset. This process continues iteratively until convergence, and points that 
converge to the same location are grouped into the same cluster.

## Output

The notebook currently detects:

```python
Number of clusters: 3
```

## Visualization

This project includes:

- Raw 3D data visualization
- Clustered 3D scatter plot
- Cluster centers highlighted separately

These visualizations help in understanding how Mean Shift identifies dense regions and
forms clusters automatically.

## Why Mean Shift?

Mean Shift is useful because:

- It does not require predefining the number of clusters
- It can detect clusters of arbitrary shape
- It is based on density estimation
- It works well for exploratory clustering tasks

## Limitations

- It can be computationally expensive on large datasets
- Performance depends heavily on bandwidth selection
- It may not perform well in very high-dimensional data

## Project Structure

```bash
day_12_mean_shift_clustering/
│── day_(ml)_mean_shift_clustering.ipynb
│── README.md
```

## Learning Outcomes

Through this project, I learned:

- How unsupervised clustering works
- The intuition behind density-based clustering
- How Mean Shift differs from centroid-based methods like K-Means
- How to visualize clusters in 3D space
- How Scikit-learn can be used for clustering implementation

## Future Improvements

- Apply Mean Shift to a real-world dataset
- Compare Mean Shift with K-Means and DBSCAN
- Experiment with different bandwidth values
- Add performance evaluation and interpretation

## Author

**Arvind**

## Note

This project is part of my ongoing daily machine learning practice series, where I 
consistently implement and document ML concepts step by step.
