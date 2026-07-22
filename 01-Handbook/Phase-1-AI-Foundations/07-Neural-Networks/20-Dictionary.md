# 📖 Neural Networks Dictionary

**Difficulty:** ⭐ Beginner–Intermediate  
**Estimated Reading Time:** 20–25 minutes  
**Prerequisites:** None (Can be used as a standalone reference)  
**Last Updated:** July 2026

---

# 📖 Introduction

This dictionary contains the most important terms used throughout the **Neural Networks** module.

Each definition is written in simple language to help beginners quickly understand technical concepts.

Use this chapter as a quick reference while studying, revising, or preparing for interviews.

---

# A

## Activation Function

A mathematical function that determines whether a neuron should produce an output. It introduces **non-linearity**, allowing Neural Networks to learn complex patterns.

**Examples:**

- ReLU
- Sigmoid
- Tanh
- Softmax

---

## Adam Optimizer

An optimization algorithm that combines ideas from **Momentum** and **RMSprop** to update model weights efficiently. It is one of the most commonly used optimizers for training Neural Networks.

---

## Artificial Neuron

The basic computational unit of a Neural Network. It receives inputs, applies weights and a bias, passes the result through an activation function, and produces an output.

---

## Autoencoder

A Neural Network that learns to compress data into a lower-dimensional representation and then reconstruct the original input. It is commonly used for compression, denoising, and anomaly detection.

---

# B

## Backpropagation

The learning algorithm used to update a Neural Network's weights by propagating prediction errors backward through the network.

---

## Batch

A small subset of the training dataset processed together before updating the model's weights.

---

## Batch Normalization

A technique that normalizes the outputs of intermediate layers during training. It helps stabilize learning and can improve training speed and generalization.

---

## Batch Size

The number of training examples processed in a single batch before the model updates its weights.

---

## Bias

An additional parameter added to the weighted sum of inputs before applying the activation function. It allows neurons to learn more flexible decision boundaries.

---

## Binary Classification

A classification task with only two possible output classes, such as **Spam** or **Not Spam**.

---

## Black Box Problem

The difficulty of understanding exactly how a Neural Network arrives at its predictions, especially in large and complex models.

---

# C

## Classification

A Machine Learning task where the model predicts one or more predefined categories.

---

## Convolution

A mathematical operation in a CNN that applies filters to an image to detect useful features such as edges, textures, and shapes.

---

## Convolutional Neural Network (CNN)

A Neural Network architecture designed primarily for image and computer vision tasks. CNNs automatically learn spatial features using convolution and pooling layers.

---

## Cross-Entropy Loss

A commonly used loss function for classification problems. It measures the difference between predicted probabilities and the true labels.

---

# D

## Data Augmentation

A technique that creates additional training examples by applying transformations such as rotation, flipping, cropping, or scaling to existing data.

---

## Decoder

The second part of an Autoencoder that reconstructs the original input from the compressed latent representation.

---

## Deep Learning

A branch of Machine Learning that uses Neural Networks with multiple hidden layers to learn complex patterns from large datasets.

---

## Dropout

A regularization technique that randomly disables neurons during training to reduce overfitting and improve generalization.

---

# E

## Early Stopping

A regularization technique that stops training when the model's performance on a validation dataset stops improving, helping prevent overfitting.

---

## Edge

In Graph Neural Networks, an edge represents a connection or relationship between two nodes.

---

## Embedding

A dense numerical representation of data such as words, sentences, or entities that captures meaningful relationships in a lower-dimensional space.

---

## Encoder

The first part of an Autoencoder that compresses input data into a latent representation.

---

## Epoch

One complete pass through the entire training dataset during the learning process.

---

# F

## Feedforward Neural Network (FNN)

The simplest Neural Network architecture in which information flows from the input layer to the output layer without loops or feedback connections.

---

## Feature

An individual measurable property or characteristic of the input data used for learning.

---

## Feature Extraction

The process of identifying useful patterns or characteristics from raw data. Neural Networks often perform this automatically.

---

## Forward Propagation

The process of passing input data through the Neural Network to generate predictions.

---

# G

## Generalization

A model's ability to make accurate predictions on unseen data rather than only the training data.

---

## Gradient

A value that indicates how much the loss function changes with respect to the model's parameters. It guides weight updates during training.

---

## Gradient Descent

An optimization algorithm that updates weights in the direction that minimizes the loss function.

---

## Graph

A data structure consisting of **nodes** and **edges**, commonly used in Graph Neural Networks.

---

## Graph Neural Network (GNN)

A Neural Network architecture designed for graph-structured data that learns from both node features and relationships between connected nodes.

---

## GRU (Gated Recurrent Unit)

A type of Recurrent Neural Network that uses update and reset gates to learn long-term dependencies more efficiently than traditional RNNs.

---

# H

## Hidden Layer

A layer located between the input and output layers where intermediate feature learning takes place.

---

## Hidden State

The memory used by RNNs, LSTMs, and GRUs to carry information from previous time steps.

---

## Hyperparameter

A setting chosen before training begins that controls how a Neural Network learns.

Examples include learning rate, batch size, and optimizer.

---

## Hyperparameter Tuning

The process of finding the best combination of hyperparameters to improve model performance.

---

# I

## Input Layer

The first layer of a Neural Network that receives the input data.

---

## Inference

The process of using a trained Neural Network to make predictions on new, unseen data.

---

## Input Gate

In an LSTM, the gate that determines how much new information should be stored in the memory cell.

---

# L

## Latent Space

A compressed representation of data learned by an Autoencoder.

---

## Layer

A collection of neurons that perform computations together within a Neural Network.

---

## Learning Rate

A hyperparameter that controls the size of weight updates during training.

---

## Leaky ReLU

An activation function similar to ReLU but allows a small gradient when the input is negative, reducing the risk of "dead" neurons.

---

## Long Short-Term Memory (LSTM)

An advanced Recurrent Neural Network architecture that uses memory cells and gates to learn long-term dependencies in sequential data.

---

## Loss Function

A mathematical function that measures how far a model's predictions are from the correct values.

---

# M

## Mean Squared Error (MSE)

A common loss function for regression problems that calculates the average squared difference between predicted and actual values.

---

## Memory Cell

The component of an LSTM responsible for storing long-term information.

---

## Message Passing

The mechanism in Graph Neural Networks where neighboring nodes exchange information to update their representations.

---

## Mini-Batch

A small subset of the training data processed during one training step.

---

## Model

A trained Neural Network that has learned patterns from data and can make predictions.

---

## Momentum

An optimization technique that accelerates Gradient Descent by considering previous weight updates.

---

# N

## Neural Network

A Machine Learning model inspired by the human brain that learns patterns from data using interconnected artificial neurons.

---

## Neuron

The basic computational unit of a Neural Network.

---

## Node

In a Graph Neural Network, a node represents an entity such as a user, product, or web page.

---

## Non-Linearity

The property introduced by activation functions that enables Neural Networks to learn complex relationships.

---

# O

## Optimizer

An algorithm that updates the model's weights to reduce prediction error during training.

---

## Output Layer

The final layer of a Neural Network that produces predictions.

---

## Overfitting

A situation where a model memorizes the training data instead of learning general patterns, resulting in poor performance on unseen data.

---

# P

## Parameter

A value learned automatically during training, such as a weight or bias.

---

## Pooling

A CNN operation that reduces the size of feature maps while preserving important information.

---

## Positional Encoding

A technique used in Transformers to provide information about the order of tokens in a sequence.

---

## Prediction

The output generated by a trained Neural Network for a given input.

---

# R

## Recurrent Neural Network (RNN)

A Neural Network architecture designed for sequential data that maintains a hidden state across time steps.

---

## Reconstruction

The process by which an Autoencoder recreates the original input from its latent representation.

---

## Regularization

Techniques used to reduce overfitting and improve a model's ability to generalize.

---

## ReLU (Rectified Linear Unit)

A widely used activation function that outputs the input if it is positive and zero otherwise.

---

## RMSprop

An optimization algorithm that adapts learning rates for individual parameters during training.

---

# S

## Self-Attention

The mechanism in Transformers that allows each token in a sequence to consider the importance of every other token in the same sequence.

---

## Sigmoid

An activation function that outputs values between 0 and 1, commonly used for binary classification.

---

## Softmax

An activation function that converts outputs into probabilities that sum to 1, commonly used for multi-class classification.

---

## Sparse Representation

A representation where many values are zero, often encouraged by L1 Regularization.

---

# T

## Tanh

An activation function that outputs values between -1 and 1.

---

## Test Dataset

A dataset used to evaluate how well a trained model performs on unseen data.

---

## Token

A basic unit of text processed by language models, such as a word, subword, or character depending on the tokenizer.

---

## Training

The process of teaching a Neural Network by updating its parameters using training data.

---

## Training Dataset

The dataset used to teach a Neural Network during the learning process.

---

## Transformer

A Neural Network architecture based on the Attention mechanism that processes sequences in parallel and powers many modern language models.

---

# U

## Underfitting

A situation where a model fails to learn important patterns from the training data, leading to poor performance on both training and unseen data.

---

# V

## Validation Dataset

A dataset used during training to monitor model performance and assist with decisions such as hyperparameter tuning and early stopping.

---

## Vanishing Gradient Problem

A training issue in deep or recurrent Neural Networks where gradients become extremely small, making it difficult for earlier layers or time steps to learn.

---

# W

## Weight

A parameter that determines the importance of an input feature in a Neural Network.

---

## Weight Initialization

The process of assigning initial values to weights before training begins.

---

# 📊 Frequently Confused Terms

| Term | Difference |
|------|------------|
| Parameter vs Hyperparameter | Parameters are learned during training; hyperparameters are chosen before training. |
| CNN vs RNN | CNNs are designed for spatial data like images, while RNNs are designed for sequential data. |
| LSTM vs GRU | Both solve long-term dependency problems; GRUs are simpler and generally faster, while LSTMs have a more complex memory mechanism. |
| Training vs Inference | Training teaches the model using labeled data; inference uses the trained model to make predictions. |
| Overfitting vs Underfitting | Overfitting memorizes the training data; underfitting fails to learn enough from it. |
| Epoch vs Batch | An epoch is one full pass through the dataset; a batch is a subset processed before updating the model. |
| Loss Function vs Optimizer | The loss function measures error, while the optimizer updates weights to reduce that error. |

---

# 📝 Final Note

Congratulations! 🎉

You have completed the **Neural Networks** module of the **AI Generalist Handbook**.

You now understand:

- Neural Network fundamentals
- Major architectures (FNN, CNN, RNN, LSTM, GRU, Autoencoder, Transformer, GNN)
- Training and optimization
- Regularization techniques
- Hyperparameter tuning
- Real-world applications
- Advantages and limitations
- Interview preparation
- Essential terminology

This knowledge forms the foundation for advanced topics such as **Computer Vision**, **Natural Language Processing**, **Generative AI**, **Large Language Models (LLMs)**, and **AI Agents**.

---

# ➡️ Next Module

# **08 – Computer Vision**

> Learn how computers interpret and understand images and videos using Neural Networks, including image classification, object detection, image segmentation, feature extraction, and modern Computer Vision applications.