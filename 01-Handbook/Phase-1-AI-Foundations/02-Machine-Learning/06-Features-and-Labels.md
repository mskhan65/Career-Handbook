# 🏷️ Features and Labels

> *"Features are the input information used by a Machine Learning model, while labels are the correct answers the model learns to predict."*

---

# 📋 Prerequisites

Before studying this topic, you should understand:

- ✅ What Machine Learning is
- ✅ How Machine Learning Works
- ✅ Machine Learning Life Cycle

---

# 🎯 Learning Goals

After completing this lesson, you will be able to:

- Understand what features are.
- Understand what labels are.
- Explain the difference between features and labels.
- Identify features and labels in real-world datasets.
- Answer interview questions related to features and labels.

---

# 📖 Introduction

Machine Learning models learn from data.

Every dataset contains information that helps the model learn patterns.

In supervised learning, data is generally divided into two parts:

- **Features (Inputs)**
- **Labels (Outputs)**

Understanding these two concepts is one of the most important fundamentals in Machine Learning.

---

# 🧠 What are Features?

**Features** are the input variables or characteristics used by a Machine Learning model to make predictions.

They describe the information about an object.

Think of features as the **questions** the model uses to find an answer.

Examples:

- Age
- Height
- Weight
- Salary
- House Size
- Number of Bedrooms
- Years of Experience

Features are also called:

- Input Variables
- Independent Variables
- Predictors

---

# 🎯 What are Labels?

A **Label** is the correct output or answer that the model is trying to learn and predict.

Think of the label as the **answer**.

Examples:

- House Price
- Email is Spam or Not Spam
- Customer Will Buy or Not
- Disease Present or Not
- Student Passed or Failed

Labels are also called:

- Target Variable
- Output Variable
- Dependent Variable

---

# 🔄 Features vs Labels

```text
Features
(Input)

Age
Salary
Experience
Education

        │
        ▼

Machine Learning Model

        │
        ▼

Label
(Output)

Will Employee Leave?
```

The model learns the relationship between the features and the label.

---

# 🌍 Real-Life Example 1

## House Price Prediction

| Features | Label |
|----------|-------|
| House Size | House Price |
| Number of Bedrooms | House Price |
| Location | House Price |
| Age of House | House Price |

Features describe the house.

The label is the selling price.

---

# 🌍 Real-Life Example 2

## Email Spam Detection

| Features | Label |
|----------|-------|
| Subject | Spam / Not Spam |
| Sender | Spam / Not Spam |
| Number of Links | Spam / Not Spam |
| Email Content | Spam / Not Spam |

The model learns from thousands of labeled emails.

---

# 🌍 Real-Life Example 3

## Student Performance

| Features | Label |
|----------|-------|
| Study Hours | Pass / Fail |
| Attendance | Pass / Fail |
| Assignment Score | Pass / Fail |
| Previous Grades | Pass / Fail |

The model predicts whether a student will pass.

---

# 💼 Business Example

## Loan Approval System

A bank wants to predict whether a customer should receive a loan.

### Features

- Age
- Income
- Employment Status
- Credit Score
- Existing Loans

↓

### Label

```text
Loan Approved

or

Loan Rejected
```

The Machine Learning model studies previous customer data and learns how these features influence the final decision.

---

# 📊 Example Dataset

| Age | Salary | Experience | Loan Approved |
|-----:|-------:|-----------:|---------------|
| 25 | 40,000 | 2 Years | No |
| 30 | 70,000 | 6 Years | Yes |
| 45 | 120,000 | 15 Years | Yes |
| 22 | 25,000 | 1 Year | No |

### Features

- Age
- Salary
- Experience

### Label

- Loan Approved

---

# 🎯 Why Features are Important

Good features help the model learn useful patterns.

Better features often lead to:

- Better predictions
- Higher accuracy
- Faster training
- Improved performance

Choosing useful features is one of the most important tasks in Machine Learning.

---

# 🎤 Interview Insight

### Question

**What is the difference between features and labels?**

### Sample Answer

> Features are the input variables used by a Machine Learning model to make predictions. Labels are the correct outputs that the model learns to predict during training. The model learns the relationship between features and labels.

---

# ⚠️ Common Beginner Mistakes

### ❌ Mistake 1

Thinking every column is a feature.

✅ **Correct**

One column is usually the label, while the remaining relevant columns are features.

---

### ❌ Mistake 2

Confusing features with labels.

✅ **Correct**

Features are inputs.

Labels are outputs.

---

### ❌ Mistake 3

Thinking more features always improve performance.

✅ **Correct**

Irrelevant features can reduce model accuracy and increase training time.

---

# 📝 Key Takeaways

- Features are the inputs used for learning.
- Labels are the outputs the model predicts.
- The model learns relationships between features and labels.
- Good features improve model performance.
- Features and labels are fundamental concepts in supervised learning.

---

# 📖 Vocabulary

| Term | Meaning |
|------|---------|
| Feature | An input variable used for prediction |
| Label | The correct output or target value |
| Input Variable | Information given to the model |
| Output Variable | The value the model predicts |
| Predictor | Another name for a feature |
| Target Variable | Another name for a label |

---

# ❓ Revision Questions

1. What is a feature?
2. What is a label?
3. What is the difference between features and labels?
4. Give three examples of features.
5. Give three examples of labels.
6. Why are features important in Machine Learning?
7. Identify the features and label in a house price prediction dataset.

---

# ⏱️ One-Minute Revision

```text
Features
↓
Input Variables

Examples
Age
Salary
Experience
House Size

        │
        ▼

Machine Learning Model

        │
        ▼

Labels
↓
Output Variables

Examples
House Price
Spam
Pass/Fail
Loan Approval

Remember

Features → Inputs

Labels → Outputs
```

---

# ➡️ Next Chapter

**07 – Training vs Testing**

> Learn why Machine Learning datasets are divided into training and testing data, and how models are evaluated before deployment.