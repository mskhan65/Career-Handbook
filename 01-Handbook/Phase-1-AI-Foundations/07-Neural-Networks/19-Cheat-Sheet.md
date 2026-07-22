# 📋 Neural Networks Cheat Sheet

**Difficulty:** ⭐ Beginner–Intermediate  
**Estimated Reading Time:** 10–15 minutes  
**Prerequisites:** Complete the Neural Networks module  
**Last Updated:** July 2026

---

# 🧠 Neural Network Definition

A **Neural Network** is a Machine Learning model inspired by the human brain that learns patterns from data by adjusting **weights** and **biases** through training.

---

# 🏗️ Basic Architecture

```text
Input Layer

↓

Hidden Layer(s)

↓

Output Layer
```

Each neuron performs:

```text
Inputs

↓

Weighted Sum

↓

+ Bias

↓

Activation Function

↓

Output
```

---

# ⚙️ Neural Network Workflow

```text
Training Data

↓

Forward Propagation

↓

Prediction

↓

Loss Function

↓

Backpropagation

↓

Optimizer Updates Weights

↓

Repeat Until Convergence
```

---

# 📚 Important Components

| Component | Purpose |
|------------|---------|
| Neuron | Basic computational unit |
| Weight | Importance assigned to an input |
| Bias | Helps shift the activation function |
| Activation Function | Adds non-linearity |
| Loss Function | Measures prediction error |
| Optimizer | Updates weights to reduce loss |
| Epoch | One complete pass through the dataset |
| Batch | Subset of training samples |
| Learning Rate | Controls weight update size |

---

# ⚡ Common Activation Functions

| Function | Typical Use |
|----------|-------------|
| ReLU | Hidden layers |
| Leaky ReLU | Hidden layers (reduces dead neurons) |
| Sigmoid | Binary classification output |
| Tanh | Hidden layers in some models |
| Softmax | Multi-class classification output |

---

# 🏛️ Neural Network Architectures

| Architecture | Best For | Key Feature |
|--------------|----------|-------------|
| Feedforward Neural Network (FNN) | Tabular Data | Simple forward flow |
| CNN | Images | Convolution & feature extraction |
| RNN | Sequential Data | Hidden state (memory) |
| LSTM | Long sequences | Memory cell & gates |
| GRU | Sequential Data | Simpler gated architecture |
| Autoencoder | Compression | Encoder–Decoder |
| Transformer | NLP & Generative AI | Self-Attention |
| Graph Neural Network (GNN) | Graph Data | Message Passing |

---

# 📊 Which Neural Network Should I Use?

```text
Tabular Data

↓

Feedforward Neural Network

----------------------------

Images

↓

CNN

----------------------------

Text

↓

Transformer

----------------------------

Speech

↓

LSTM / GRU / Transformer

----------------------------

Time-Series

↓

LSTM / GRU

----------------------------

Recommendation Systems

↓

Graph Neural Network

----------------------------

Social Networks

↓

Graph Neural Network

----------------------------

Image Compression

↓

Autoencoder
```

---

# 🖼️ CNN Pipeline

```text
Image

↓

Convolution

↓

Feature Maps

↓

Pooling

↓

Flatten

↓

Fully Connected Layer

↓

Prediction
```

---

# 🔄 RNN Pipeline

```text
Input Sequence

↓

Hidden State

↺

↓

Output Sequence
```

---

# 🧠 LSTM Memory Flow

```text
Previous Memory

↓

Forget Gate

↓

Input Gate

↓

Memory Cell

↓

Output Gate

↓

Next Hidden State
```

---

# ⚡ GRU Memory Flow

```text
Previous State

↓

Update Gate

↓

Reset Gate

↓

New Hidden State
```

---

# 🤖 Transformer Pipeline

```text
Input

↓

Embeddings

↓

Positional Encoding

↓

Self-Attention

↓

Feedforward Network

↓

Output
```

---

# 🕸️ Graph Neural Network Pipeline

```text
Node

↓

Receive Neighbor Information

↓

Message Passing

↓

Update Node Representation

↓

Prediction
```

---

# 🗜️ Autoencoder Pipeline

```text
Input

↓

Encoder

↓

Latent Space

↓

Decoder

↓

Reconstructed Output
```

---

# 📈 Training Process

```text
Initialize Weights

↓

Forward Propagation

↓

Calculate Loss

↓

Backpropagation

↓

Optimizer

↓

Update Weights

↓

Repeat
```

---

# 🎯 Loss Functions

| Task | Common Loss Function |
|------|----------------------|
| Regression | Mean Squared Error (MSE) |
| Binary Classification | Binary Cross-Entropy |
| Multi-class Classification | Categorical Cross-Entropy |

---

# 🚀 Popular Optimizers

| Optimizer | Characteristics |
|-----------|-----------------|
| SGD | Simple Gradient Descent |
| Momentum | Faster convergence than SGD |
| RMSprop | Adaptive learning rates |
| Adam | Combines Momentum and RMSprop (most widely used) |

---

# 🛡️ Regularization Techniques

| Technique | Purpose |
|-----------|---------|
| Dropout | Randomly disables neurons |
| L1 Regularization | Encourages sparse weights |
| L2 Regularization | Penalizes large weights |
| Early Stopping | Stops before overfitting |
| Data Augmentation | Increases training data diversity |
| Batch Normalization | Stabilizes training |

---

# ⚙️ Important Hyperparameters

- Learning Rate
- Batch Size
- Epochs
- Optimizer
- Number of Hidden Layers
- Number of Neurons
- Activation Function
- Dropout Rate
- Weight Initialization

---

# 🔍 Hyperparameter Tuning Methods

| Method | Description |
|---------|-------------|
| Manual Search | Trial and error |
| Grid Search | Tests every predefined combination |
| Random Search | Tests random combinations |
| Bayesian Optimization | Uses previous results to choose promising combinations |

---

# 🌍 Real-World Applications

| Industry | Application |
|----------|-------------|
| Healthcare | Disease detection, medical imaging |
| Finance | Fraud detection, risk assessment |
| Retail | Product recommendations |
| Manufacturing | Defect detection |
| Transportation | Self-driving cars |
| Agriculture | Crop disease detection |
| Cybersecurity | Threat detection |
| NLP | Translation, chatbots |
| Generative AI | Text, image, code generation |
| Scientific Research | Drug discovery, climate modeling |

---

# ✅ Advantages

- Learns complex patterns
- High accuracy
- Automatic feature learning
- Works with multiple data types
- Scalable
- Supports automation
- Wide industry adoption

---

# ⚠️ Limitations

- Requires large datasets
- High computational cost
- Long training time
- Black Box nature
- Risk of overfitting
- Sensitive to data quality
- Difficult hyperparameter tuning
- Ethical concerns

---

# ⚖️ Architecture Comparison

| Architecture | Data Type | Memory | Best Use |
|--------------|-----------|---------|----------|
| FNN | Tabular | ❌ | Classification, Regression |
| CNN | Images | ❌ | Computer Vision |
| RNN | Sequential | ✅ | Time-Series, Text |
| LSTM | Sequential | ✅ Long-term | Speech, Forecasting |
| GRU | Sequential | ✅ Long-term | Efficient sequence modeling |
| Autoencoder | Any | N/A | Compression, Denoising |
| Transformer | Text & Sequences | Attention | NLP, Generative AI |
| GNN | Graph | Neighbor Information | Recommendations, Fraud Detection |

---

# ⚠️ Common Beginner Mistakes

❌ Thinking Neural Networks always outperform simpler models.

❌ Confusing parameters with hyperparameters.

❌ Believing more layers always improve accuracy.

❌ Ignoring overfitting.

❌ Choosing the wrong architecture for the data.

❌ Using an inappropriate learning rate.

❌ Training without validation data.

---

# 🎤 Interview Quick Facts

- CNNs are best for images.
- Transformers dominate modern NLP and Generative AI.
- GNNs are designed for graph-structured data.
- LSTMs and GRUs address the Vanishing Gradient Problem.
- Dropout helps reduce overfitting.
- Adam is one of the most commonly used optimizers.
- Hyperparameters are chosen before training.
- Parameters are learned during training.
- Self-Attention is the foundation of Transformers.
- Message Passing is the core mechanism of GNNs.

---

# 📝 Quick Formula Sheet

### Neuron

```text
Output = Activation((Inputs × Weights) + Bias)
```

---

### Learning Loop

```text
Prediction

↓

Loss

↓

Gradient

↓

Weight Update
```

---

### General Training Cycle

```text
Data

↓

Forward Propagation

↓

Loss

↓

Backpropagation

↓

Optimizer

↓

Updated Model
```

---

# 🚀 Memory Map

```text
Neural Networks

│

├── Architecture
│     ├── Input Layer
│     ├── Hidden Layer
│     └── Output Layer
│
├── Components
│     ├── Weights
│     ├── Biases
│     ├── Activation Functions
│     ├── Loss Function
│     └── Optimizer
│
├── Architectures
│     ├── FNN
│     ├── CNN
│     ├── RNN
│     ├── LSTM
│     ├── GRU
│     ├── Autoencoder
│     ├── Transformer
│     └── GNN
│
├── Training
│     ├── Forward Propagation
│     ├── Backpropagation
│     ├── Gradient Descent
│     └── Hyperparameter Tuning
│
├── Regularization
│     ├── Dropout
│     ├── L1
│     ├── L2
│     ├── Early Stopping
│     └── Data Augmentation
│
└── Applications
      ├── Healthcare
      ├── Finance
      ├── Retail
      ├── Transportation
      ├── Cybersecurity
      ├── NLP
      ├── Generative AI
      └── Scientific Research
```

---

# 🎯 Final Exam Tips

Before moving to the next module, ensure you can confidently explain:

- ✅ What is a Neural Network?
- ✅ How Forward Propagation works.
- ✅ How Backpropagation updates weights.
- ✅ Why activation functions are necessary.
- ✅ The difference between CNN, RNN, LSTM, GRU, Transformer, Autoencoder, and GNN.
- ✅ How regularization reduces overfitting.
- ✅ The role of hyperparameter tuning.
- ✅ Real-world applications of each architecture.
- ✅ The advantages and limitations of Neural Networks.
- ✅ Which architecture is appropriate for different types of data.

---

# ➡️ Next Chapter

**20 – Dictionary**

> Review all important Neural Network terminology with concise definitions, making it easy to refresh key concepts and technical vocabulary before interviews, exams, or starting the next AI module.