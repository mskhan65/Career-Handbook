# 📚 Deep Learning Dictionary

**Difficulty:** ⭐ Beginner  
**Estimated Reading Time:** 15–20 minutes  
**Prerequisites:** None (Can be used alongside the entire Deep Learning module)  
**Last Updated:** July 2026

---

# 📖 Introduction

This dictionary contains the most important Deep Learning terms covered throughout this module.

Use it as a quick reference while:

- 📚 Studying
- 💼 Preparing for interviews
- 📝 Revising for exams
- 🚀 Building AI projects

The definitions are written in simple, beginner-friendly language.

---

# 🔤 A

## Activation Function

A mathematical function that determines the output of a neuron and introduces **non-linearity**, allowing neural networks to learn complex patterns.

**Example:**

ReLU, Sigmoid, Tanh, Softmax

---

## Adam

A popular optimizer that combines ideas from **Momentum** and **RMSprop** to train neural networks efficiently.

---

## Artificial Intelligence (AI)

The broad field of creating machines that can perform tasks requiring human intelligence.

```text
AI

↓

Machine Learning

↓

Deep Learning
```

---

## Artificial Neuron

The basic building block of a neural network.

It receives inputs, applies weights and a bias, uses an activation function, and produces an output.

---

# 🔤 B

## Backpropagation

The algorithm that sends prediction errors backward through a neural network to calculate how weights and biases should be updated.

---

## Batch Gradient Descent

A type of Gradient Descent that updates the model's parameters after processing the entire training dataset.

---

## Bias

A trainable value added to the weighted sum of inputs before applying the activation function.

Bias gives neurons additional flexibility when learning patterns.

---

## Binary Classification

A classification problem with only **two possible outcomes**.

Examples:

- Spam / Not Spam
- Fraud / Not Fraud
- Yes / No

---

## Binary Cross-Entropy

A loss function commonly used for binary classification problems.

---

# 🔤 C

## Categorical Cross-Entropy

A loss function commonly used for **multi-class classification** problems.

---

## Classification

A Machine Learning task where the goal is to predict categories or labels.

Examples:

- Cat or Dog
- Healthy or Sick
- Positive or Negative

---

## Computational Cost

The amount of computing resources (time, memory, and processing power) required to train or run a model.

---

## Computer Vision

A field of AI that enables computers to understand images and videos.

---

## Convergence

The stage during training where the model's performance stops improving significantly because the loss has become very low or stabilized.

---

# 🔤 D

## Data

The information used to train or evaluate AI models.

Examples:

- Images
- Text
- Audio
- Videos
- Sensor readings

---

## Deep Learning

A subset of Machine Learning that uses neural networks with multiple hidden layers to automatically learn patterns from data.

---

## Deployment

The process of making a trained AI model available for real-world use.

---

# 🔤 E

## Epoch

One complete pass of the entire training dataset through the neural network during training.

---

## Error

The difference between a model's prediction and the correct answer.

The Loss Function measures this error.

---

# 🔤 F

## Feature

An individual piece of information used by a model to make predictions.

Examples:

- Age
- Income
- Pixel value
- Temperature

---

## Feature Learning

The process by which Deep Learning automatically discovers useful patterns from raw data.

---

## Forward Propagation

The process of passing input data through a neural network to generate a prediction.

---

# 🔤 G

## Generative AI

A branch of AI that creates new content such as text, images, audio, video, or code.

---

## Gradient

A value that indicates how a model's parameters should change to reduce the loss.

---

## Gradient Descent

An optimization algorithm that updates weights and biases to minimize the loss.

---

## GPU (Graphics Processing Unit)

A specialized processor that accelerates Deep Learning training by performing many calculations simultaneously.

---

# 🔤 H

## Hidden Layer

A layer located between the input and output layers where the neural network learns patterns and representations.

---

## Hyperparameter

A value that is set before training begins and controls the learning process.

Examples:

- Learning rate
- Batch size
- Number of epochs

---

# 🔤 I

## Inference

The process of using a trained model to make predictions on new, unseen data.

---

## Input Layer

The first layer of a neural network that receives input data.

---

## Iteration

One update of the model's parameters during training. Depending on the batch size, multiple iterations may occur within a single epoch.

---

# 🔤 L

## Learning Rate

A value that controls how much the model updates its weights during each training step.

---

## Leaky ReLU

An activation function similar to ReLU that allows a small negative output instead of returning zero for all negative inputs.

---

## Loss

A numerical measure of how far the model's prediction is from the correct answer.

Lower loss generally indicates better performance during training.

---

## Loss Function

A mathematical function that calculates the prediction error.

---

# 🔤 M

## Machine Learning

A subset of Artificial Intelligence in which systems learn patterns from data rather than relying solely on explicitly programmed rules.

---

## Mean Absolute Error (MAE)

A regression loss function that measures the average absolute difference between predicted and actual values.

---

## Mean Squared Error (MSE)

A regression loss function that measures the average squared difference between predicted and actual values.

---

## Mini-Batch Gradient Descent

A Gradient Descent method that updates the model after processing a small group (mini-batch) of training examples.

---

## Model

A trained mathematical representation that makes predictions from input data.

---

## Momentum

An optimizer that uses previous updates to help accelerate learning and reduce unnecessary oscillations.

---

## Multi-Class Classification

A classification problem with more than two possible classes.

Examples:

- Cat
- Dog
- Bird

---

# 🔤 N

## Neural Network

A collection of interconnected artificial neurons organized into layers that learn patterns from data.

---

## Neural Network Architecture

The structure of a neural network, including the number of layers, neurons, and how they are connected.

---

## Node

Another name for an artificial neuron.

---

## Non-Linearity

The property that enables neural networks to learn complex relationships beyond straight-line patterns.

Activation functions introduce non-linearity.

---

# 🔤 O

## Optimizer

An algorithm that updates a model's weights and biases to reduce the loss.

Examples:

- SGD
- Momentum
- RMSprop
- Adam

---

## Output Layer

The final layer of a neural network that produces predictions.

---

## Overfitting

A situation where a model memorizes the training data instead of learning general patterns, leading to poor performance on new data.

---

# 🔤 P

## Parameter

A trainable value in a neural network, such as a weight or bias.

---

## Perceptron

The simplest artificial neuron, introduced by Frank Rosenblatt in 1958, designed for linear classification problems.

---

## Prediction

The output generated by a neural network after processing input data.

---

# 🔤 R

## Regression

A Machine Learning task where the goal is to predict continuous numerical values.

Examples:

- House prices
- Temperature
- Sales

---

## ReLU (Rectified Linear Unit)

A widely used activation function that outputs:

- 0 for negative inputs
- The input value for positive inputs

---

## RMSprop

An optimizer that adapts the learning rate for each parameter during training.

---

# 🔤 S

## Sigmoid

An activation function that produces outputs between **0 and 1**, making it useful for binary classification outputs.

---

## Softmax

An activation function commonly used for multi-class classification.

It converts outputs into probabilities that sum to 1.

---

## Stochastic Gradient Descent (SGD)

A version of Gradient Descent that updates the model after processing one training example at a time.

---

## Supervised Learning

A Machine Learning approach where the model learns from labeled data.

Deep Learning models can also be trained using supervised learning.

---

# 🔤 T

## Tanh (Hyperbolic Tangent)

An activation function that produces outputs between **-1 and 1**.

---

## Test Data

A dataset used to evaluate how well a trained model performs on unseen data.

---

## Training

The process of teaching a neural network by updating its weights and biases using data.

---

## Training Data

The dataset used to teach a model during training.

---

## TPU (Tensor Processing Unit)

A specialized processor designed to accelerate Machine Learning and Deep Learning workloads.

---

# 🔤 V

## Validation Data

A separate dataset used during training to monitor model performance and help tune model settings before final evaluation.

---

# 🔤 W

## Weight

A trainable value that determines the importance of an input feature in a neural network.

Weights are adjusted during training to improve predictions.

---

# 📚 Quick Reference Table

| Term | Simple Meaning |
|------|----------------|
| Deep Learning | Learning using deep neural networks |
| Neural Network | Connected artificial neurons |
| Neuron | Basic processing unit |
| Weight | Importance of an input |
| Bias | Additional adjustable value |
| Activation Function | Decides a neuron's output |
| Forward Propagation | Makes predictions |
| Loss Function | Measures prediction error |
| Backpropagation | Learns from mistakes |
| Gradient Descent | Reduces prediction error |
| Optimizer | Updates weights efficiently |
| Training | Teaching the model |
| Inference | Using the model |
| ReLU | Most common hidden-layer activation |
| Sigmoid | Binary classification output |
| Softmax | Multi-class classification output |
| Adam | Popular optimizer |
| Epoch | One full pass through the training dataset |
| Overfitting | Memorizing instead of generalizing |
| GPU | Hardware for faster Deep Learning |
| TPU | Hardware specialized for AI workloads |

---

# 🎯 Memory Tips

```text
AI

↓

Machine Learning

↓

Deep Learning

↓

Neural Network

↓

Neuron

↓

Weights + Bias

↓

Activation Function

↓

Prediction

↓

Loss Function

↓

Backpropagation

↓

Gradient Descent

↓

Optimizer

↓

Better Model
```

---

# 📝 Key Takeaways

- Deep Learning terminology builds on a small set of core ideas.
- Understanding these terms makes it easier to read research papers, documentation, and technical interviews.
- Focus first on the relationship between neurons, weights, activation functions, loss functions, Backpropagation, and optimizers.
- Revisit this dictionary whenever you encounter unfamiliar terminology while studying advanced AI topics.

---

# 🎉 Module Complete

Congratulations! 🎉

You have successfully completed the **06 – Deep Learning** module.

You now understand:

- ✅ Deep Learning fundamentals
- ✅ Neural networks and artificial neurons
- ✅ Activation functions
- ✅ Forward and Backpropagation
- ✅ Loss functions
- ✅ Gradient Descent and optimizers
- ✅ Training vs inference
- ✅ Applications of Deep Learning
- ✅ Advantages and limitations
- ✅ Key terminology

You are now ready to begin the next module:

> **07 – Neural Networks**, where you'll explore neural network architectures, specialized network types (CNNs, RNNs, Transformers, etc.), and the building blocks behind modern AI systems.