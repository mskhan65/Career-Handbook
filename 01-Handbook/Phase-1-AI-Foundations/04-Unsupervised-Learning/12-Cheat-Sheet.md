# 📄 Unsupervised Learning Cheat Sheet

> **Quick Revision Guide**  
> Use this cheat sheet for last-minute revision before interviews, exams, or practical Machine Learning projects.

---

# 🎯 Unsupervised Learning

**Definition**

A type of Machine Learning where a model learns from **unlabeled data** to discover hidden patterns, structures, relationships, or groups without being given the correct answers.

---

# 🧠 Basic Workflow

```text
Unlabeled Data
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
Analyze Results
      │
      ▼
Use Insights
```

---

# 📚 Key Terms

| Term | Meaning |
|------|---------|
| Unsupervised Learning | Learning from unlabeled data |
| Feature | Input variable |
| Unlabeled Data | Data without correct output labels |
| Cluster | Group of similar data points |
| Similarity | Degree to which data points resemble each other |
| Pattern | Hidden relationship in data |
| Dimension | A feature or input variable |
| Outlier | A data point that differs significantly from others |

---

# 🔀 Types of Unsupervised Learning

```text
Unsupervised Learning
        │
 ┌──────┴──────┐
 ▼             ▼

Clustering   Dimensionality
             Reduction
```

---

# 📂 Clustering

### Purpose

Group similar data points together.

### Goal

Discover natural groups in data.

### Common Algorithms

- K-Means
- Hierarchical Clustering
- DBSCAN
- Mean Shift

### Common Applications

- Customer Segmentation
- Product Grouping
- Community Detection
- Market Basket Analysis
- Image Organization

---

# 📉 Dimensionality Reduction

### Purpose

Reduce the number of features while preserving important information.

### Goal

Simplify large and complex datasets.

### Common Techniques

- Principal Component Analysis (PCA)
- t-SNE
- UMAP

### Common Applications

- Data Visualization
- Image Compression
- Feature Reduction
- Faster Model Training
- Noise Reduction

---

# ⚖️ Clustering vs Dimensionality Reduction

| Clustering | Dimensionality Reduction |
|------------|--------------------------|
| Groups similar data | Reduces the number of features |
| Produces clusters | Produces fewer dimensions |
| Used for segmentation | Used for preprocessing and visualization |
| Focuses on similarity | Focuses on preserving information |

---

# 🤖 Common Algorithms

| Algorithm | Category | Main Purpose |
|-----------|----------|--------------|
| K-Means | Clustering | Groups data into **K** clusters |
| Hierarchical Clustering | Clustering | Builds a hierarchy of clusters |
| DBSCAN | Clustering | Finds density-based clusters and detects outliers |
| Mean Shift | Clustering | Finds clusters in dense regions |
| PCA | Dimensionality Reduction | Reduces features |
| t-SNE | Dimensionality Reduction | Visualizes high-dimensional data |
| UMAP | Dimensionality Reduction | Reduces dimensions while preserving structure |

---

# 🌍 Real-World Applications

| Industry | Example |
|----------|---------|
| Retail | Customer Segmentation |
| Banking | Fraud Investigation |
| Healthcare | Patient Grouping |
| Marketing | Target Audience Analysis |
| E-commerce | Product Recommendations |
| Manufacturing | Machine Monitoring |
| Transportation | Route Analysis |
| Social Media | Community Detection |
| Scientific Research | Pattern Discovery |
| Computer Vision | Image Organization |

---

# 🌟 Advantages

- Works with unlabeled data
- Discovers hidden patterns
- Supports data exploration
- Enables customer segmentation
- Detects unusual patterns
- Reduces data complexity
- Improves decision-making

---

# ⚠️ Limitations

- No correct answers for validation
- Difficult to evaluate results
- Requires human interpretation
- Sensitive to data quality
- Choosing the right algorithm can be challenging
- Some algorithms are computationally expensive
- Some discovered patterns may not be meaningful

---

# 💼 Business Examples

| Business Problem | Solution |
|------------------|----------|
| Customer Segmentation | K-Means |
| Fraud Investigation | DBSCAN |
| Product Recommendations | Clustering |
| Patient Grouping | Hierarchical Clustering |
| Image Compression | PCA |
| Data Visualization | PCA, t-SNE, UMAP |
| Feature Reduction | PCA |

---

# 📊 Algorithm Selection Guide

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

Need Detect Outliers?

        │
        ▼
      DBSCAN

----------------------

Need Reduce Features?

        │
        ▼
        PCA

----------------------

Need Visualize Data?

        │
        ▼
     t-SNE / UMAP
```

---

# 🎤 Interview Quick Facts

### What is Unsupervised Learning?

Learning from **unlabeled data** to discover hidden patterns.

---

### Two Main Types

- Clustering
- Dimensionality Reduction

---

### Common Clustering Algorithms

- K-Means
- Hierarchical Clustering
- DBSCAN
- Mean Shift

---

### Common Dimensionality Reduction Techniques

- PCA
- t-SNE
- UMAP

---

### Common Applications

- Customer Segmentation
- Recommendation Systems
- Market Basket Analysis
- Fraud Investigation
- Healthcare
- Scientific Research
- Image Organization

---

# 🚀 Workflow Summary

```text
Unlabeled Data
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
Business Insights
```

---

# 📝 Memory Map

```text
Unsupervised Learning
        │
        ▼
Uses Unlabeled Data
        │
        ▼
Discover Hidden Patterns
        │
        ├──────────────┐
        ▼              ▼

Clustering     Dimensionality
               Reduction

        │              │
        ▼              ▼

K-Means         PCA
Hierarchical    t-SNE
DBSCAN          UMAP
Mean Shift
```

---

# 🎯 Exam Tips

- Remember that **Unsupervised Learning uses unlabeled data**.
- Understand the difference between **Clustering** and **Dimensionality Reduction**.
- Know when to use **K-Means**, **Hierarchical Clustering**, **DBSCAN**, and **PCA**.
- Support answers with real-world business examples.
- Explain both the **advantages** and **limitations** of Unsupervised Learning.

---

# ⚡ 30-Second Revision

```text
Unsupervised Learning

↓

Uses Unlabeled Data

↓

No Correct Answers

↓

Discover Hidden Patterns

↓

Two Main Types

Clustering
↓

K-Means
Hierarchical
DBSCAN
Mean Shift

Dimensionality Reduction
↓

PCA
t-SNE
UMAP

Applications

Customer Segmentation
Fraud Investigation
Healthcare
Recommendation Systems
Image Organization

Remember

Find Patterns

↓

Group Data

or

Reduce Features

↓

Generate Business Insights
```

---

# ➡️ Next Chapter

**13 – Dictionary**

> A glossary of important Unsupervised Learning terms and definitions for quick reference and long-term retention.