# 🤖 Common Unsupervised Learning Algorithms

> *"Different Unsupervised Learning algorithms solve different types of problems. Some group similar data into clusters, while others reduce the number of features to simplify complex datasets."*

---

# 📋 Prerequisites

Before studying this topic, you should understand:

- ✅ What Unsupervised Learning is
- ✅ How Unsupervised Learning Works
- ✅ Clustering
- ✅ Dimensionality Reduction

---

# 🎯 Learning Goals

After completing this lesson, you will be able to:

- Identify the most common Unsupervised Learning algorithms.
- Understand the purpose of each algorithm.
- Compare different algorithms.
- Recognize real-world applications.
- Explain when to use each algorithm.

---

# 📖 Introduction

There is no single algorithm that works best for every Unsupervised Learning problem.

Some algorithms are designed to:

- Group similar data points.
- Detect unusual observations.
- Reduce the number of features.
- Simplify high-dimensional datasets.

Choosing the right algorithm depends on:

- The type of data
- The business problem
- The desired outcome

---

# 🌳 Common Unsupervised Learning Algorithms

```text
Unsupervised Learning
          │
 ┌────────┴────────┐
 ▼                 ▼
Clustering   Dimensionality
Algorithms     Reduction
                    │
                    ▼
                  PCA
```

---

# 1️⃣ K-Means Clustering

## What is K-Means?

**K-Means** is one of the most popular Clustering algorithms.

It divides data into **K clusters**, where **K** is chosen before training.

Each data point is assigned to the cluster with the nearest center (called a **centroid**).

---

## How K-Means Works

```text
Choose K Clusters
        │
        ▼
Place Initial Centroids
        │
        ▼
Assign Data Points
        │
        ▼
Update Centroids
        │
        ▼
Repeat Until Stable
```

---

## Example

A shopping mall wants to divide customers into **3 groups**.

The algorithm automatically creates:

```text
Cluster 1

Young
High Spending
```

```text
Cluster 2

Middle Income
Moderate Spending
```

```text
Cluster 3

High Income
Low Spending
```

---

## Applications

- Customer Segmentation
- Market Analysis
- Product Grouping
- Image Compression

---

## Advantages

- Easy to understand.
- Fast on large datasets.
- Works well with well-separated clusters.

---

## Limitations

- The value of **K** must be chosen in advance.
- Sensitive to outliers.
- Works best with roughly spherical clusters.

---

# 2️⃣ Hierarchical Clustering

## What is Hierarchical Clustering?

Hierarchical Clustering builds a hierarchy of clusters instead of creating all clusters at once.

The results are often displayed as a tree-like diagram called a **dendrogram**.

---

## How It Works

```text
Every Data Point
Starts as Its Own Cluster
          │
          ▼
Merge Similar Clusters
          │
          ▼
Repeat Until
One Large Cluster
```

---

## Example

```text
Customer A

Customer B

↓

Merge

Customer C

↓

Merge

Final Hierarchy
```

---

## Applications

- Biology
- Gene Analysis
- Document Organization
- Customer Segmentation

---

## Advantages

- No need to specify the number of clusters beforehand.
- Produces a visual hierarchy of clusters.

---

## Limitations

- Computationally expensive for very large datasets.
- Once clusters are merged, they cannot be separated later in the process.

---

# 3️⃣ DBSCAN

## What is DBSCAN?

**DBSCAN (Density-Based Spatial Clustering of Applications with Noise)** groups data based on **density**.

It identifies dense regions as clusters and labels isolated points as **outliers (noise)**.

---

## How It Works

```text
Dense Region

● ● ● ● ●

↓

Cluster

Sparse Points

      ●

↓

Outlier
```

---

## Applications

- Fraud Detection
- GPS Data Analysis
- Image Processing
- Anomaly Detection

---

## Advantages

- Does not require choosing the number of clusters beforehand.
- Can discover clusters with irregular shapes.
- Detects outliers automatically.

---

## Limitations

- Performance depends on selecting appropriate density parameters.
- Can struggle when cluster densities vary significantly.

---

# 4️⃣ Principal Component Analysis (PCA)

## What is PCA?

**Principal Component Analysis (PCA)** is the most common Dimensionality Reduction technique.

Instead of grouping data, PCA reduces the number of features while preserving as much variation in the data as possible.

---

## How PCA Works

```text
Original Dataset

10 Features

        │
        ▼

Analyze Relationships

        │
        ▼

Create Principal Components

        │
        ▼

3 Features
```

The new features (called **principal components**) summarize the original information.

---

## Applications

- Data Visualization
- Image Compression
- Feature Extraction
- Data Preprocessing

---

## Advantages

- Reduces dataset complexity.
- Improves computational efficiency.
- Makes visualization easier.

---

## Limitations

- Reduced features are harder to interpret.
- Some information may be lost during transformation.

---

# 📊 Algorithm Comparison

| Algorithm | Category | Main Purpose |
|-----------|----------|--------------|
| K-Means | Clustering | Groups data into **K** clusters |
| Hierarchical Clustering | Clustering | Builds a hierarchy of clusters |
| DBSCAN | Clustering | Finds clusters based on data density and detects outliers |
| PCA | Dimensionality Reduction | Reduces the number of features |

---

# 🌍 Real-World Applications

| Industry | Algorithm | Example |
|----------|-----------|---------|
| Retail | K-Means | Customer Segmentation |
| Banking | DBSCAN | Fraud Detection |
| Healthcare | Hierarchical Clustering | Patient Grouping |
| Marketing | K-Means | Target Audience Analysis |
| Computer Vision | PCA | Image Compression |
| Scientific Research | PCA | Data Visualization |
| Cybersecurity | DBSCAN | Network Anomaly Detection |

---

# 💼 Business Example

An e-commerce company wants to better understand its customers.

**Problem 1:** Group customers with similar buying behavior.

**Solution:** K-Means Clustering

---

**Problem 2:** Detect unusual purchasing activity.

**Solution:** DBSCAN

---

**Problem 3:** Simplify a dataset with hundreds of customer attributes.

**Solution:** PCA

---

# 📊 Choosing the Right Algorithm

```text
Need Customer Groups?

        │
        ▼
     K-Means

----------------------

Need Cluster Hierarchy?

        │
        ▼
Hierarchical Clustering

----------------------

Need Outlier Detection?

        │
        ▼
      DBSCAN

----------------------

Need Fewer Features?

        │
        ▼
        PCA
```

---

# 🎤 Interview Insight

### Question

**Name some common Unsupervised Learning algorithms.**

### Sample Answer

> Common Unsupervised Learning algorithms include K-Means Clustering, Hierarchical Clustering, DBSCAN, and Principal Component Analysis (PCA). K-Means groups data into a fixed number of clusters, Hierarchical Clustering builds a hierarchy of clusters, DBSCAN identifies dense clusters and outliers, and PCA reduces the number of features while preserving important information.

---

# ⚠️ Common Beginner Mistakes

### ❌ Mistake 1

Thinking every Unsupervised Learning algorithm creates clusters.

✅ **Correct**

Algorithms like PCA reduce dimensions instead of creating clusters.

---

### ❌ Mistake 2

Believing K-Means automatically knows the best number of clusters.

✅ **Correct**

The value of **K** must usually be chosen before training.

---

### ❌ Mistake 3

Confusing PCA with a Clustering algorithm.

✅ **Correct**

PCA performs Dimensionality Reduction; it does not group data into clusters.

---

# 📝 Key Takeaways

- Different algorithms solve different Unsupervised Learning problems.
- K-Means groups data into a predefined number of clusters.
- Hierarchical Clustering creates a tree-like hierarchy of clusters.
- DBSCAN groups data based on density and identifies outliers.
- PCA reduces the number of features while preserving important information.

---

# 📖 Vocabulary

| Term | Meaning |
|------|---------|
| K-Means | A clustering algorithm that divides data into **K** clusters |
| Centroid | The center point of a cluster in K-Means |
| Hierarchical Clustering | A clustering method that builds a hierarchy of clusters |
| Dendrogram | A tree-like diagram showing hierarchical cluster relationships |
| DBSCAN | A density-based clustering algorithm that detects outliers |
| Density | The concentration of data points within a region |
| Outlier | A data point that differs significantly from most others |
| PCA | A Dimensionality Reduction technique that creates principal components |
| Principal Component | A new feature created by PCA that summarizes the original data |

---

# ❓ Revision Questions

1. Name four common Unsupervised Learning algorithms.
2. What is the purpose of K-Means?
3. What is a centroid in K-Means?
4. How does Hierarchical Clustering differ from K-Means?
5. What is DBSCAN mainly used for?
6. What is PCA, and why is it used?
7. Which algorithm is best for reducing the number of features?

---

# ⏱️ One-Minute Revision

```text
Common Algorithms

↓

K-Means
↓

Group Data into K Clusters

----------------------

Hierarchical Clustering
↓

Build Cluster Hierarchy

----------------------

DBSCAN
↓

Density-Based Clustering

↓

Detect Outliers

----------------------

PCA
↓

Reduce Features

↓

Simplify Dataset

Remember

Group Data

↓

K-Means
Hierarchical
DBSCAN

Reduce Features

↓

PCA
```

---

# ➡️ Next Chapter

**08 – Applications**

> Explore how Unsupervised Learning is used across industries such as healthcare, finance, retail, cybersecurity, marketing, manufacturing, and scientific research to uncover hidden patterns and generate valuable insights.