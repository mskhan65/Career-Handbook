# 👜 Bag of Words (BoW)

**Difficulty:** ⭐ Beginner  
**Estimated Reading Time:** 30–35 minutes  
**Prerequisites:** 01 – Introduction to NLP, 02 – What is NLP?, 03 – Text Preprocessing, 04 – Tokenization, 05 – Stemming and Lemmatization  
**Last Updated:** July 2026

---

# 📖 Introduction

Computers cannot understand words directly.

Machine Learning algorithms work with **numbers**, not text.

For example, consider the sentence:

```text
I love AI.
```

A human immediately understands its meaning.

A computer simply sees characters.

To apply Machine Learning, we must convert text into numerical features.

One of the earliest and simplest methods for doing this is called the **Bag of Words (BoW)** model.

Although modern NLP often uses **Word Embeddings** and **Transformers**, Bag of Words remains an important foundational concept because it introduces the idea of converting text into numerical vectors.

---

# 🎯 Learning Goals

After completing this chapter, you will be able to:

- Understand what the Bag of Words model is.
- Learn how text is converted into numbers.
- Build a vocabulary from a collection of documents.
- Create BoW vectors.
- Understand the advantages and limitations of BoW.
- Explore real-world applications.

---

# 🤔 What is Bag of Words?

**Bag of Words (BoW)** is a text representation technique that converts text into numerical vectors by counting how many times each word appears.

The model treats a document as a **bag of words**, meaning:

- Word order is ignored.
- Grammar is ignored.
- Only the frequency of words matters.

Example:

```text
I love AI.

AI loves me.
```

Both sentences contain similar words.

BoW focuses on **which words appear** and **how often**, rather than the order in which they appear.

---

# 🎯 Why is Bag of Words Needed?

Machine Learning models cannot process raw text.

BoW converts text into a numerical format suitable for Machine Learning algorithms.

Workflow:

```text
Text

↓

Tokenization

↓

Vocabulary

↓

Word Counts

↓

Numerical Vector

↓

Machine Learning Model
```

---

# 🏗️ Step 1 – Collect Documents

Suppose we have three documents.

```text
Document 1

I love AI
```

```text
Document 2

AI is amazing
```

```text
Document 3

I love Machine Learning
```

---

# 🏗️ Step 2 – Text Preprocessing

After preprocessing:

```text
Document 1

love ai
```

```text
Document 2

ai amazing
```

```text
Document 3

love machine learning
```

Notice that common words such as **I** and **is** have been removed for simplicity.

---

# 🏗️ Step 3 – Build the Vocabulary

Collect every unique word.

```text
amazing

ai

learning

love

machine
```

This list is called the **vocabulary**.

---

# 🏗️ Step 4 – Count Word Frequencies

Now count how many times each vocabulary word appears in every document.

| Vocabulary | Doc 1 | Doc 2 | Doc 3 |
|------------|------:|------:|------:|
| amazing | 0 | 1 | 0 |
| ai | 1 | 1 | 0 |
| learning | 0 | 0 | 1 |
| love | 1 | 0 | 1 |
| machine | 0 | 0 | 1 |

Each row represents one vocabulary word.

Each column represents one document.

---

# 🏗️ Step 5 – Create Numerical Vectors

Document 1:

```text
love ai
```

Vector:

```text
[0, 1, 0, 1, 0]
```

---

Document 2:

```text
ai amazing
```

Vector:

```text
[1, 1, 0, 0, 0]
```

---

Document 3:

```text
love machine learning
```

Vector:

```text
[0, 0, 1, 1, 1]
```

Now each document is represented using numbers.

These vectors can be used as input to Machine Learning models.

---

# ⚙️ Complete BoW Workflow

```text
Raw Documents

↓

Text Preprocessing

↓

Tokenization

↓

Vocabulary Creation

↓

Count Word Frequency

↓

Vector Representation

↓

Machine Learning Algorithm
```

---

# 📦 Example with Two Sentences

Sentence 1:

```text
Cats chase mice.
```

Sentence 2:

```text
Dogs chase cats.
```

Vocabulary:

```text
cats

chase

dogs

mice
```

Vectors:

| Word | Sentence 1 | Sentence 2 |
|------|-----------:|-----------:|
| cats | 1 | 1 |
| chase | 1 | 1 |
| dogs | 0 | 1 |
| mice | 1 | 0 |

---

# 🧩 Why is it Called a "Bag" of Words?

Imagine placing all the words into a bag.

```text
Sentence

↓

Words

↓

Bag
```

The model remembers:

- Which words exist
- How many times they appear

It **does not remember**:

- Word order
- Grammar
- Sentence structure

Example:

```text
Dog bites man.
```

and

```text
Man bites dog.
```

Both contain the same words.

A simple BoW representation may produce identical or nearly identical vectors, even though the meanings are very different.

This is one of the biggest limitations of BoW.

---

# 🌍 Real-World Example 1 — Spam Detection

Emails:

```text
Win money now
```

```text
Meeting tomorrow
```

After BoW:

```text
Word Counts

↓

Machine Learning

↓

Spam

or

Not Spam
```

---

# 🌍 Real-World Example 2 — Sentiment Analysis

Customer Review:

```text
This phone is excellent.
```

BoW counts words like:

```text
excellent

phone
```

The Machine Learning model uses these counts to predict whether the review is positive, negative, or neutral.

---

# 🌍 Real-World Example 3 — News Classification

News headline:

```text
Stock market rises today.
```

BoW converts the headline into a numerical vector.

The classifier predicts:

- Business
- Sports
- Politics
- Technology

---

# 💼 Business Example

## Customer Feedback Analysis

A company receives thousands of customer reviews every day.

Pipeline:

```text
Customer Reviews

↓

Text Preprocessing

↓

Tokenization

↓

Bag of Words

↓

Machine Learning

↓

Positive

Negative

Neutral
```

### Business Benefits

- Faster review analysis
- Better customer insights
- Improved products
- Automated reporting

---

# 📊 Advantages of Bag of Words

- Easy to understand
- Simple to implement
- Fast to compute
- Works well for small datasets
- Effective baseline for text classification

---

# ⚠️ Limitations of Bag of Words

- Ignores word order
- Ignores grammar
- Ignores context
- Produces sparse vectors
- Vocabulary grows very large
- Cannot understand synonyms
- Cannot understand semantic meaning

---

# 📊 Bag of Words vs Raw Text

| Raw Text | Bag of Words |
|----------|--------------|
| Human-readable | Numerical vectors |
| Contains grammar | Ignores grammar |
| Preserves word order | Ignores word order |
| Rich contextual meaning | Only word frequencies |

---

# 📊 Bag of Words vs Word Embeddings

| Bag of Words | Word Embeddings |
|--------------|-----------------|
| Counts word frequency | Learns word meaning |
| Ignores context | Captures semantic relationships |
| Sparse vectors | Dense vectors |
| Larger vocabulary | Better generalization |
| Simple | More powerful |

---

# 📊 Bag of Words vs TF-IDF

| Bag of Words | TF-IDF |
|--------------|--------|
| Uses raw word counts | Weights words by importance |
| Common words may dominate | Common words receive lower importance |
| Simpler | More informative for many tasks |

You will learn **TF-IDF** in the next chapter.

---

# 🎤 Interview Insight

### Question

**What is the Bag of Words model?**

### Sample Answer

> Bag of Words (BoW) is a text representation technique that converts documents into numerical vectors by counting how many times each word appears. It ignores grammar and word order, focusing only on word frequency. BoW is simple, efficient, and widely used as a baseline technique for text classification and other Machine Learning tasks.

---

# ⚠️ Common Beginner Mistakes

### ❌ Mistake 1

Thinking Bag of Words understands language.

✅ **Correct**

BoW only counts words. It does not understand grammar, meaning, or context.

---

### ❌ Mistake 2

Believing word order matters.

✅ **Correct**

BoW ignores the order of words.

---

### ❌ Mistake 3

Assuming larger word counts always mean more importance.

✅ **Correct**

Frequently occurring words are not always the most informative. Techniques such as TF-IDF help address this limitation.

---

### ❌ Mistake 4

Thinking Bag of Words is obsolete.

✅ **Correct**

Although modern NLP often uses embeddings and Transformers, BoW is still useful for learning, rapid prototyping, and some traditional Machine Learning applications.

---

# 📝 Key Takeaways

- Bag of Words converts text into numerical vectors using word frequencies.
- It begins by building a vocabulary from the dataset.
- Each document is represented by counting occurrences of vocabulary words.
- BoW ignores grammar, context, and word order.
- Despite its limitations, it remains an important foundational technique in NLP.

---

# 📖 Vocabulary

| Term | Meaning |
|------|---------|
| Bag of Words (BoW) | Text representation based on word frequencies |
| Vocabulary | List of all unique words in a dataset |
| Word Frequency | Number of times a word appears in a document |
| Document | A single text sample such as an email, review, or article |
| Corpus | A collection of documents |
| Sparse Vector | A vector containing many zero values |
| Feature Vector | Numerical representation of a document |
| Text Representation | Converting text into a numerical format for AI models |
| Token | A word, subword, sentence, or character produced during tokenization |
| Corpus Vocabulary | Combined set of unique tokens across all documents |

---

# ❓ Revision Questions

1. What is the Bag of Words model?
2. Why is Bag of Words used in NLP?
3. What is a vocabulary?
4. How are BoW vectors created?
5. Why is it called a "Bag" of Words?
6. What information does BoW ignore?
7. What are the main advantages of BoW?
8. What are the limitations of BoW?
9. Compare Bag of Words and Word Embeddings.
10. How does Bag of Words help Machine Learning models process text?

---

# ⏱️ One-Minute Revision

```text
Raw Text

↓

Text Preprocessing

↓

Tokenization

↓

Vocabulary

↓

Count Word Frequencies

↓

Bag of Words Vector

↓

Machine Learning Model

↓

Prediction

Key Characteristics

✔ Simple
✔ Fast
✔ Numerical Representation

Limitations

✘ Ignores Word Order
✘ Ignores Grammar
✘ Ignores Context
✘ Sparse Vectors

Applications

Spam Detection

Sentiment Analysis

News Classification

Document Classification
```

---

# ➡️ Next Chapter

**07 – TF-IDF (Term Frequency–Inverse Document Frequency)**

> Learn how TF-IDF improves on Bag of Words by assigning higher importance to informative words and reducing the influence of very common words across documents.