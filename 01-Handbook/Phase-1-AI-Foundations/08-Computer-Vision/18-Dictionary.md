# 📖 Computer Vision Dictionary

**Difficulty:** ⭐ Beginner to ⭐⭐⭐ Intermediate  
**Estimated Reading Time:** 20–25 minutes  
**Prerequisites:** None  
**Last Updated:** July 2026

---

# 📚 Introduction

This dictionary contains the most important Computer Vision terms covered throughout this module.

Each definition is written in simple, beginner-friendly language to help you quickly understand and remember essential concepts.

Use this chapter as a reference while studying, preparing for interviews, or revising Computer Vision topics.

---

# A

## Accuracy

The percentage of correct predictions made by a model out of all predictions.

**Example:**

If a model correctly classifies 95 out of 100 images, its accuracy is **95%**.

---

## Activation Function

A mathematical function that introduces non-linearity into a neural network, enabling it to learn complex patterns.

**Example:**

ReLU, Sigmoid, and Tanh.

---

## Adversarial Attack

A technique where small, carefully designed changes are made to an image to trick an AI model into making incorrect predictions.

---

## Artificial Intelligence (AI)

A branch of computer science focused on building systems that can perform tasks that normally require human intelligence.

---

## Augmentation

Another name for **Data Augmentation**, where training images are transformed to create additional examples without changing their labels.

---

# B

## Batch

A small group of training images processed together before updating the model's parameters.

---

## Batch Size

The number of training samples processed in one iteration during model training.

---

## Bias

A systematic error that causes a model to perform unfairly or inaccurately for certain groups or situations, often due to unrepresentative training data.

---

## Bounding Box

A rectangular box used in Object Detection to indicate the location of an object in an image.

```text
+-------------+
|     Dog     |
+-------------+
```

---

# C

## Classification

The task of assigning one or more labels to an image.

---

## Color Channel

One component of a color image.

For RGB images:

- Red
- Green
- Blue

---

## Computer Vision

A field of Artificial Intelligence that enables computers to understand and analyze images and videos.

---

## Convolution

The operation of sliding a filter (kernel) across an image to detect visual features.

---

## Convolutional Neural Network (CNN)

A Deep Learning model specifically designed for image analysis and other visual tasks.

---

## Crop

Removing part of an image while keeping the remaining region.

---

# D

## Data Augmentation

Creating additional training images by applying transformations such as rotation, flipping, cropping, or brightness adjustment.

---

## Dataset

A collection of images used for training, validating, or testing AI models.

---

## Deep Learning

A subset of Machine Learning that uses neural networks with many layers to learn complex patterns.

---

## Dice Coefficient

A metric used to measure the similarity between predicted and actual segmentation masks.

---

# E

## Edge Detection

A technique used to identify object boundaries by detecting sharp intensity changes in an image.

---

## Embedding

A numerical vector that represents important information about an object, such as a face.

---

## Epoch

One complete pass through the entire training dataset during model training.

---

# F

## Face Detection

The process of locating faces within an image.

---

## Face Embedding

A numerical representation of a face used to compare facial similarity.

---

## Face Identification

Finding the identity of a person by comparing one face against many stored identities (1:N matching).

---

## Face Recognition

Identifying or verifying a person's identity using facial features.

---

## Face Verification

Confirming whether a person's face matches a claimed identity (1:1 matching).

---

## False Acceptance Rate (FAR)

The percentage of unauthorized users who are incorrectly accepted by a recognition system.

---

## False Rejection Rate (FRR)

The percentage of authorized users who are incorrectly rejected by a recognition system.

---

## Feature

A meaningful visual pattern, such as an edge, texture, or shape, that helps identify objects.

---

## Feature Extraction

The process of identifying useful visual information from images.

---

## Feature Map

The output produced after applying a convolution filter to an image.

---

## Filter (Kernel)

A small matrix of learnable values used in convolution to detect visual patterns.

---

## Fine-Tuning

Training selected layers of a pre-trained model so it performs better on a new dataset.

---

## Flatten

Converting multi-dimensional feature maps into a one-dimensional vector before classification.

---

# G

## Grayscale Image

An image that contains only shades of gray rather than color.

---

## Ground Truth

The correct labels or annotations used as the reference when training or evaluating AI models.

---

# H

## HOG (Histogram of Oriented Gradients)

A traditional feature extraction method that describes objects using edge directions.

---

# I

## Image Classification

Assigning a label to an entire image.

---

## Image Processing

Techniques used to improve or modify images before analysis.

---

## Image Segmentation

Labeling every pixel in an image so that objects and regions are identified precisely.

---

## ImageNet

A large image dataset commonly used for training Computer Vision models.

---

## Instance Segmentation

A segmentation technique that distinguishes each individual object separately.

---

## Intersection over Union (IoU)

A metric that measures how much the predicted region overlaps with the true region.

---

# K

## Kernel

Another name for a **Filter** used during convolution.

---

# L

## Label

The correct category assigned to an image or object.

---

## Learning Rate

A hyperparameter that controls how much model parameters change during each training step.

---

# M

## mAP (Mean Average Precision)

A common evaluation metric used for Object Detection models.

---

## Machine Learning

A subset of AI where computers learn patterns from data instead of following explicitly programmed rules.

---

## Model

A trained algorithm that makes predictions based on input data.

---

# N

## Neural Network

A machine learning model inspired by the structure of the human brain, consisting of interconnected artificial neurons.

---

## Noise

Unwanted variations or distortions in an image that can reduce model performance.

---

## Normalization

Scaling pixel values to a standard range to improve model training.

---

# O

## Object Detection

Detecting both the class and location of objects in an image.

---

## Occlusion

When part of an object is hidden or blocked by another object.

---

## Offline Data Augmentation

Generating augmented images before training begins.

---

## Online Data Augmentation

Generating augmented images dynamically during training.

---

## ORB (Oriented FAST and Rotated BRIEF)

A fast traditional feature extraction algorithm used for object matching and tracking.

---

# P

## Panoptic Segmentation

A segmentation technique that combines Semantic Segmentation and Instance Segmentation into one unified task.

---

## Pixel

The smallest unit of a digital image.

---

## Pixel Accuracy

The percentage of correctly classified pixels in an image segmentation task.

---

## Pooling

Reducing the size of feature maps while preserving important information.

---

## Precision

The proportion of predicted positive results that are actually correct.

---

## Prediction

The output produced by a trained AI model.

---

## Pre-trained Model

A model that has already been trained on a large dataset and can be reused for other tasks.

---

# R

## Recall

The proportion of actual positive cases that are correctly identified.

---

## ReLU (Rectified Linear Unit)

An activation function defined as:

```text
ReLU(x) = max(0, x)
```

---

## Resolution

The number of pixels in an image, typically expressed as width × height.

---

## RGB

A color model based on three channels:

- Red
- Green
- Blue

---

## Rotation

A Data Augmentation technique that turns an image by a specified angle.

---

# S

## SAM (Segment Anything Model)

A foundation model developed by Meta AI that can generate segmentation masks for a wide variety of objects with minimal prompting.

---

## Scaling

Changing the size of an image while maintaining its proportions.

---

## Semantic Segmentation

Assigning the same class label to every pixel belonging to the same object category.

---

## Softmax

An activation function that converts model outputs into probabilities that sum to 1.

---

## SURF (Speeded-Up Robust Features)

A traditional feature extraction algorithm for detecting and describing local image features.

---

## SIFT (Scale-Invariant Feature Transform)

A classic feature extraction algorithm that detects distinctive image keypoints and descriptors.

---

# T

## Texture

The visual pattern or surface appearance of an object, used as a feature for recognition.

---

## Transfer Learning

Reusing knowledge from a pre-trained model for a new but related task.

---

# U

## U-Net

A CNN architecture widely used for medical image segmentation.

---

# V

## Validation Dataset

A dataset used during training to evaluate model performance and tune hyperparameters without updating model weights.

---

## Video Analytics

Using Computer Vision techniques to automatically analyze video streams for events, objects, or activities.

---

# W

## Weight

A learnable parameter in a neural network that determines the importance of an input during prediction.

---

# Y

## YOLO (You Only Look Once)

A family of real-time Object Detection models known for balancing speed and accuracy.

---

# 📋 Commonly Used Terms

| Term | Meaning |
|------|---------|
| AI | Artificial Intelligence |
| CV | Computer Vision |
| CNN | Convolutional Neural Network |
| RGB | Red, Green, Blue |
| IoU | Intersection over Union |
| mAP | Mean Average Precision |
| FAR | False Acceptance Rate |
| FRR | False Rejection Rate |
| HOG | Histogram of Oriented Gradients |
| ORB | Oriented FAST and Rotated BRIEF |
| SIFT | Scale-Invariant Feature Transform |
| SURF | Speeded-Up Robust Features |
| SAM | Segment Anything Model |

---

# 📝 Key Takeaways

- Computer Vision terminology forms the foundation for understanding image analysis and Deep Learning.
- Concepts such as CNNs, Object Detection, Image Segmentation, and Transfer Learning are essential for modern Computer Vision.
- Metrics like Accuracy, IoU, mAP, Dice Coefficient, FAR, and FRR are commonly used to evaluate model performance.
- Traditional feature extraction methods (SIFT, SURF, HOG, ORB) remain important historical concepts, while CNN-based approaches dominate modern applications.
- Keeping a strong vocabulary helps in interviews, certifications, and real-world AI projects.

---

# 🎓 Congratulations!

🎉 You have successfully completed the **08 – Computer Vision** module of the **AI Generalist Handbook**.

You now understand:

- ✅ Fundamentals of Computer Vision
- ✅ Digital Images and Pixels
- ✅ Image Processing Basics
- ✅ Image Classification
- ✅ Object Detection
- ✅ Image Segmentation
- ✅ Face Recognition
- ✅ Feature Extraction
- ✅ CNNs in Computer Vision
- ✅ Transfer Learning
- ✅ Data Augmentation
- ✅ Real-World Applications
- ✅ Advantages and Limitations
- ✅ Interview Preparation
- ✅ Revision and Cheat Sheet
- ✅ Essential Computer Vision Vocabulary

---

# 🚀 Next Module

# **09 – Natural Language Processing (NLP)**

In the next module, you will learn how AI understands, processes, and generates human language.

Topics include:

- Text preprocessing
- Tokenization
- Stemming and Lemmatization
- Bag of Words
- TF-IDF
- Word Embeddings
- RNNs for NLP
- Transformers
- Attention Mechanism
- BERT
- GPT
- NLP Applications
- Sentiment Analysis
- Machine Translation
- Question Answering
- Named Entity Recognition (NER)
- Interview Questions
- Revision
- Cheat Sheet
- Dictionary

**Next Stop:** 🌐 **09 – Natural Language Processing**