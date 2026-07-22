# 📄 Computer Vision Cheat Sheet

**Difficulty:** ⭐ Beginner to ⭐⭐⭐ Intermediate  
**Estimated Reading Time:** 10–15 minutes  
**Prerequisites:** Complete Computer Vision Module  
**Last Updated:** July 2026

---

# 🧠 What is Computer Vision?

**Computer Vision (CV)** is a branch of Artificial Intelligence (AI) that enables computers to interpret, analyze, and understand images and videos.

### Goal

```text
Image / Video

↓

Computer Vision

↓

Understanding

↓

Decision
```

---

# 📊 Computer Vision Pipeline

```text
Image / Video

↓

Image Acquisition

↓

Preprocessing

↓

Feature Extraction

↓

Deep Learning Model

↓

Prediction

↓

Decision
```

---

# 🖼️ Digital Images

A digital image is made up of **pixels**.

```text
Image

↓

Pixels

↓

Numbers

↓

AI Processes Numbers
```

### RGB Image

```text
Red

Green

Blue
```

---

# 🛠️ Image Processing

### Common Operations

- Resize
- Crop
- Normalize
- Grayscale Conversion
- Noise Reduction
- Filtering
- Rotation
- Flipping

**Purpose**

- Improve image quality
- Standardize inputs
- Prepare data for AI models

---

# 🎯 Core Computer Vision Tasks

```text
Computer Vision

│

├── Image Classification

├── Object Detection

├── Image Segmentation

├── Face Recognition

└── Feature Extraction
```

---

# 🏷️ Image Classification

### Goal

Assign **one label** to an image.

```text
Image

↓

Cat
```

Examples:

- Animal recognition
- Food classification
- Medical diagnosis

---

# 📍 Object Detection

### Goal

Locate and classify multiple objects.

```text
Image

↓

Bounding Boxes

↓

Car

Person

Dog
```

Examples:

- Self-driving cars
- Security cameras
- Warehouse automation

---

# 🧩 Image Segmentation

### Goal

Label **every pixel**.

### Types

```text
Semantic

↓

Instance

↓

Panoptic
```

Examples:

- Medical imaging
- Autonomous vehicles
- Agriculture

---

# 😊 Face Recognition

### Pipeline

```text
Image

↓

Face Detection

↓

Face Alignment

↓

Feature Extraction

↓

Face Embedding

↓

Database Comparison

↓

Identity
```

Applications:

- Face Unlock
- Banking
- Airports
- Attendance

---

# 🔍 Feature Extraction

### Hierarchy

```text
Edges

↓

Corners

↓

Textures

↓

Shapes

↓

Object Parts

↓

Objects
```

Traditional Methods:

- SIFT
- SURF
- HOG
- ORB

Modern Method:

- CNNs automatically learn features.

---

# 🧠 CNN Architecture

```text
Input

↓

Convolution

↓

ReLU

↓

Pooling

↓

Convolution

↓

Pooling

↓

Flatten

↓

Fully Connected

↓

Softmax

↓

Prediction
```

---

# ⚙️ CNN Components

| Component | Purpose |
|-----------|---------|
| Input | Receives image |
| Convolution | Learns image features |
| Filter (Kernel) | Detects patterns |
| Feature Map | Output of convolution |
| ReLU | Adds non-linearity |
| Pooling | Reduces feature map size |
| Flatten | Converts feature maps into a vector |
| Fully Connected | Performs classification |
| Softmax | Produces probabilities |

---

# 🔄 Transfer Learning

### Workflow

```text
Pre-trained Model

↓

Feature Extraction

or

Fine-Tuning

↓

New Task
```

### Popular Models

- ResNet
- EfficientNet
- MobileNet
- DenseNet
- VGG
- Inception
- ConvNeXt

### Benefits

- Less data
- Faster training
- Better accuracy
- Lower cost

---

# 🎨 Data Augmentation

### Common Techniques

```text
Flip

Rotate

Crop

Scale

Translate

Brightness

Contrast

Color Jitter

Noise

Random Erasing
```

### Benefits

- Reduces overfitting
- Improves robustness
- Increases dataset diversity
- Improves generalization

---

# 📏 Evaluation Metrics

## Classification

| Metric | Purpose |
|---------|---------|
| Accuracy | Overall correctness |
| Precision | Correct positive predictions |
| Recall | Finds actual positives |
| F1-score | Balance of Precision and Recall |

---

## Object Detection

| Metric | Purpose |
|---------|---------|
| IoU | Bounding box overlap |
| mAP | Overall detection performance |

---

## Image Segmentation

| Metric | Purpose |
|---------|---------|
| Pixel Accuracy | Correctly classified pixels |
| IoU | Region overlap |
| Dice Coefficient | Segmentation similarity |

---

## Face Recognition

| Metric | Purpose |
|---------|---------|
| FAR | False Acceptance Rate |
| FRR | False Rejection Rate |

---

# 📊 Important Comparisons

## Classification vs Detection

| Classification | Detection |
|---------------|-----------|
| One label | Multiple objects |
| No location | Bounding boxes |

---

## Detection vs Segmentation

| Detection | Segmentation |
|-----------|--------------|
| Bounding boxes | Pixel labels |
| Approximate location | Exact boundaries |

---

## Semantic vs Instance Segmentation

| Semantic | Instance |
|----------|----------|
| Same label for all objects | Distinguishes each object |

---

## Face Detection vs Face Recognition

| Detection | Recognition |
|-----------|-------------|
| Finds faces | Identifies people |

---

## Feature Extraction vs Transfer Learning

| Feature Extraction | Transfer Learning |
|-------------------|-------------------|
| Learns visual patterns | Reuses learned knowledge |

---

## Feature Extraction vs Fine-Tuning

| Feature Extraction | Fine-Tuning |
|-------------------|-------------|
| Freeze layers | Retrain selected layers |

---

## Online vs Offline Augmentation

| Online | Offline |
|--------|---------|
| During training | Before training |

---

# 🌍 Major Applications

- Healthcare
- Autonomous Vehicles
- Retail
- Manufacturing
- Agriculture
- Banking
- Security
- Sports Analytics
- Entertainment
- Logistics
- Robotics
- Environmental Monitoring

---

# ✅ Advantages

- Automation
- High speed
- High accuracy
- Scalability
- Continuous operation
- Improved safety
- Lower operational costs
- Better decision-making
- Real-time processing

---

# ⚠️ Limitations

- Large datasets required
- High computational cost
- Sensitive to image quality
- Environmental variations
- Bias in training data
- Privacy concerns
- Security risks
- Limited contextual understanding
- Ethical challenges

---

# 📝 Important Formulas

## ReLU

```text
ReLU(x) = max(0, x)
```

---

## Accuracy

```text
Accuracy

=

Correct Predictions

/

Total Predictions
```

---

## Precision

```text
Precision

=

TP

/

(TP + FP)
```

---

## Recall

```text
Recall

=

TP

/

(TP + FN)
```

---

## F1-score

```text
F1

=

2 × (Precision × Recall)

/

(Precision + Recall)
```

---

# 🎤 Interview Keywords

Remember these important terms:

- Computer Vision
- Pixel
- RGB
- CNN
- Convolution
- Filter (Kernel)
- Feature Map
- ReLU
- Pooling
- Flatten
- Softmax
- Image Classification
- Object Detection
- Image Segmentation
- Face Recognition
- Feature Extraction
- Transfer Learning
- Fine-Tuning
- Data Augmentation
- IoU
- mAP
- Dice Coefficient
- FAR
- FRR

---

# 🚀 Complete Workflow

```text
Image

↓

Image Processing

↓

Feature Extraction

↓

CNN

↓

Convolution

↓

ReLU

↓

Pooling

↓

Flatten

↓

Fully Connected Layer

↓

Prediction

↓

Applications

Healthcare

Retail

Manufacturing

Agriculture

Transportation

Security

↓

Improve Performance

Transfer Learning

+

Data Augmentation

↓

Evaluate

Accuracy

Precision

Recall

F1-score

IoU

mAP

Dice

FAR

FRR
```

---

# ⚡ One-Minute Cheat Sheet

```text
Computer Vision

↓

Tasks

├── Classification
├── Detection
├── Segmentation
├── Face Recognition
└── Feature Extraction

↓

CNN

Input

↓

Convolution

↓

ReLU

↓

Pooling

↓

Flatten

↓

Fully Connected

↓

Softmax

↓

Prediction

↓

Improve Model

├── Transfer Learning
└── Data Augmentation

↓

Metrics

Classification

Accuracy

Precision

Recall

F1

Detection

IoU

mAP

Segmentation

Pixel Accuracy

IoU

Dice

Recognition

FAR

FRR

↓

Applications

Healthcare

Retail

Manufacturing

Agriculture

Transportation

Security

Robotics

Logistics
```

---

# ➡️ Next Chapter

**18 – Dictionary**

> A comprehensive glossary of Computer Vision terminology, including definitions for image processing, CNNs, segmentation, transfer learning, evaluation metrics, and other essential concepts used throughout this module.