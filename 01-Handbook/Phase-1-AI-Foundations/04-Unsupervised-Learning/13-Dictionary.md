# 📖 Unsupervised Learning Dictionary

> **Glossary of Terms**  
> This dictionary contains the most important terms used in **Unsupervised Learning**. Keep it as a quick reference while studying or working on Machine Learning projects.

---

# A

## Algorithm

A step-by-step procedure that enables a computer to learn patterns from data and solve a specific problem.

### Example

K-Means is an algorithm used for clustering.

---

## Anomaly

A data point that is significantly different from the majority of the dataset.

### Example

A customer who usually spends **$50** suddenly makes a **$10,000** purchase.

---

## Anomaly Detection

The process of identifying unusual or unexpected data points that differ from normal patterns.

### Common Uses

- Fraud investigation
- Network security
- Equipment monitoring

---

# C

## Centroid

The center point of a cluster in the K-Means algorithm.

Each data point is assigned to the nearest centroid.

---

## Cluster

A group of similar data points.

### Example

Customers with similar shopping behavior may belong to the same cluster.

---

## Clustering

An Unsupervised Learning technique that groups similar data points into clusters.

### Common Algorithms

- K-Means
- Hierarchical Clustering
- DBSCAN
- Mean Shift

---

# D

## Data Exploration

The process of analyzing a dataset to understand its structure, patterns, and relationships before building Machine Learning models.

---

## Dataset

A collection of related data organized into rows and columns.

---

## DBSCAN

**Density-Based Spatial Clustering of Applications with Noise**

A clustering algorithm that forms clusters based on data density and identifies isolated data points as outliers.

---

## Dimension

Another name for a feature or input variable.

### Example

Age, Salary, and Height are dimensions.

---

## Dimensionality Reduction

An Unsupervised Learning technique that reduces the number of features while preserving important information.

---

## Distance Measure

A mathematical way to determine how similar or different two data points are.

Common distance measures include:

- Euclidean Distance
- Manhattan Distance
- Cosine Distance (or Cosine Similarity)

---

# E

## Euclidean Distance

The straight-line distance between two data points.

It is commonly used in clustering algorithms such as K-Means.

---

# F

## Feature

An individual input variable used to describe a data point.

### Example

| Person | Features |
|---------|----------|
| Customer | Age, Income, Spending Score |

---

## Feature Reduction

Reducing the number of input features while preserving useful information.

PCA is a common feature reduction technique.

---

# H

## Hierarchical Clustering

A clustering algorithm that builds a hierarchy of clusters by merging or splitting data points.

The results are often shown using a dendrogram.

---

# K

## K-Means

A clustering algorithm that divides data into **K** predefined clusters by assigning data points to the nearest centroid.

---

# L

## Label

The correct output or target value associated with a data point.

### Example

| Image | Label |
|--------|-------|
| Cat Image | Cat |

Unsupervised Learning does **not** use labels during training.

---

## Labeled Data

Data that contains both input features and correct output labels.

Labeled data is primarily used in **Supervised Learning**.

---

# M

## Mean Shift

A clustering algorithm that identifies clusters by locating regions with high data density without requiring the number of clusters in advance.

---

## Model

A trained Machine Learning system that learns patterns from data to perform specific tasks.

---

# N

## Noise

Random, irrelevant, or incorrect data that can interfere with learning and reduce the quality of results.

### Examples

- Typographical errors
- Sensor errors
- Duplicate records
- Missing values

---

# O

## Outlier

A data point that differs significantly from most other data points in a dataset.

Outliers may indicate:

- Rare events
- Errors
- Unusual behavior

---

# P

## Pattern

A meaningful relationship or structure discovered within data.

---

## Pattern Discovery

The process of identifying hidden relationships, trends, or structures in data.

---

## PCA (Principal Component Analysis)

A Dimensionality Reduction technique that transforms many features into a smaller set of principal components while preserving as much variation as possible.

---

## Preprocessing

Preparing data before training a Machine Learning model.

Common preprocessing tasks include:

- Handling missing values
- Removing duplicates
- Scaling features
- Cleaning incorrect data

---

## Principal Component

A new feature created by PCA that combines information from multiple original features while capturing as much variation as possible.

---

# S

## Similarity

A measure of how closely two data points resemble each other.

Higher similarity generally means the points are more likely to belong to the same cluster.

---

## Structure

The hidden organization or relationships present within a dataset.

Unsupervised Learning attempts to discover this structure automatically.

---

# T

## t-SNE

**t-Distributed Stochastic Neighbor Embedding**

A Dimensionality Reduction technique mainly used to visualize high-dimensional datasets in two or three dimensions.

---

# U

## UMAP

**Uniform Manifold Approximation and Projection**

A Dimensionality Reduction technique used for visualization while preserving both local and global relationships in the data.

---

## Unlabeled Data

Data that contains input features but no correct output labels.

### Example

| Age | Income | Spending Score |
|------|---------|----------------|
| 25 | $40,000 | 80 |

There is no target column.

---

## Unsupervised Learning

A type of Machine Learning where a model learns from unlabeled data to discover hidden patterns, structures, similarities, or relationships without being given the correct answers.

---

# V

## Variance

A measure of how much the values in a dataset differ from one another.

PCA aims to preserve as much variance as possible when reducing dimensions.

---

## Visualization

The graphical representation of data to make patterns easier to understand.

Dimensionality Reduction techniques such as PCA, t-SNE, and UMAP are commonly used for visualization.

---

# W

## Workflow

The sequence of steps followed when solving a Machine Learning problem.

Typical Unsupervised Learning workflow:

```text
Collect Data
      │
      ▼
Prepare Data
      │
      ▼
Choose Algorithm
      │
      ▼
Discover Patterns
      │
      ▼
Interpret Results
      │
      ▼
Apply Insights
```

---

# 🔤 Common Abbreviations

| Abbreviation | Full Form |
|--------------|-----------|
| AI | Artificial Intelligence |
| ML | Machine Learning |
| PCA | Principal Component Analysis |
| DBSCAN | Density-Based Spatial Clustering of Applications with Noise |
| t-SNE | t-Distributed Stochastic Neighbor Embedding |
| UMAP | Uniform Manifold Approximation and Projection |

---

# 📚 Most Important Terms to Remember

| Term | Quick Meaning |
|------|---------------|
| Unsupervised Learning | Learning from unlabeled data |
| Cluster | Group of similar data points |
| Clustering | Grouping similar data |
| Feature | Input variable |
| Dimension | Another name for a feature |
| Pattern | Hidden relationship in data |
| Outlier | Unusual data point |
| Centroid | Center of a cluster |
| PCA | Reduces the number of features |
| DBSCAN | Detects density-based clusters and outliers |
| K-Means | Creates **K** clusters |
| Hierarchical Clustering | Builds a hierarchy of clusters |
| Mean Shift | Finds clusters based on data density |
| t-SNE | Visualizes high-dimensional data |
| UMAP | Reduces dimensions while preserving data structure |

---

# 🎯 Final Revision

```text
Unsupervised Learning

↓

Uses Unlabeled Data

↓

Discovers Hidden Patterns

↓

Two Main Types

↓

Clustering
&
Dimensionality Reduction

↓

Common Algorithms

K-Means
Hierarchical Clustering
DBSCAN
Mean Shift
PCA
t-SNE
UMAP

↓

Applications

Customer Segmentation
Fraud Investigation
Recommendation Systems
Healthcare
Scientific Research
Image Organization

↓

Goal

Find Structure

↓

Generate Insights

↓

Support Better Decisions
```

---

# 🎉 Congratulations!

You have successfully completed the **Unsupervised Learning** chapter.

You now understand:

- ✅ What Unsupervised Learning is
- ✅ How it works
- ✅ Types of Unsupervised Learning
- ✅ Clustering
- ✅ Dimensionality Reduction
- ✅ Common algorithms
- ✅ Real-world applications
- ✅ Advantages and limitations
- ✅ Interview questions
- ✅ Key terminology

You are now ready to continue with the next major topic:

# ➡️ Next Module

**05 – Reinforcement Learning**

> Learn how intelligent agents make decisions by interacting with an environment, receiving rewards or penalties, and improving their behavior through trial and error.