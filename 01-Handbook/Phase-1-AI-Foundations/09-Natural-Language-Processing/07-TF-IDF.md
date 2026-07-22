# 📊 TF-IDF (Term Frequency – Inverse Document Frequency)

**Difficulty:** ⭐⭐ Beginner to Intermediate  
**Estimated Reading Time:** 35–40 minutes  
**Prerequisites:** 01 – Introduction to NLP, 02 – What is NLP?, 03 – Text Preprocessing, 04 – Tokenization, 05 – Stemming and Lemmatization, 06 – Bag of Words  
**Last Updated:** July 2026

---

# 📖 Introduction

In the previous chapter, you learned about the **Bag of Words (BoW)** model.

BoW counts how many times each word appears in a document.

However, not all words are equally important.

Consider two words:

```text
the
```

and

```text
artificial
```

The word **"the"** appears in almost every document.

The word **"artificial"** appears much less frequently and carries more useful information.

Bag of Words treats both words equally if they occur the same number of times.

To solve this problem, NLP uses **TF-IDF (Term Frequency–Inverse Document Frequency)**.

TF-IDF gives **higher importance to informative words** and **lower importance to very common words**.

---

# 🎯 Learning Goals

After completing this chapter, you will be able to:

- Understand why TF-IDF was developed.
- Learn the concepts of Term Frequency (TF).
- Learn the concepts of Inverse Document Frequency (IDF).
- Understand how TF-IDF scores are calculated.
- Compare TF-IDF with Bag of Words.
- Explore real-world applications of TF-IDF.

---

# 🤔 Why Do We Need TF-IDF?

Imagine two documents.

### Document 1

```text
The movie was amazing.
```

### Document 2

```text
The weather is amazing today.
```

Words like:

```text
the

is

was
```

appear frequently.

Words like:

```text
movie

weather
```

provide much more information.

Bag of Words simply counts occurrences.

TF-IDF recognizes that common words should contribute less than unique, informative words.

---

# 📖 What is TF-IDF?

**TF-IDF (Term Frequency–Inverse Document Frequency)** is a numerical technique used to measure how important a word is to a document within a collection of documents (called a corpus).

It combines two ideas:

```text
TF

×

IDF

=

TF-IDF Score
```

A word receives a **high TF-IDF score** if:

- It appears frequently in one document.
- It appears in only a few documents across the corpus.

---

# 🧩 Components of TF-IDF

```text
TF-IDF

│

├── Term Frequency (TF)

└── Inverse Document Frequency (IDF)
```

---

# 1️⃣ Term Frequency (TF)

**Term Frequency (TF)** measures how often a word appears in a document.

Example:

Document:

```text
AI is amazing.

AI changes the world.
```

Word counts:

| Word | Frequency |
|------|----------:|
| AI | 2 |
| amazing | 1 |
| changes | 1 |
| world | 1 |

Higher frequency means a higher TF value.

A simple TF calculation is:

```text
TF = Number of times a word appears in a document
```

Some implementations normalize this count by the total number of words in the document.

---

# 2️⃣ Inverse Document Frequency (IDF)

Some words appear in almost every document.

Examples:

- the
- is
- and
- of

These words are not very useful for distinguishing one document from another.

**Inverse Document Frequency (IDF)** reduces the importance of such common words.

Concept:

```text
Rare Word

↓

High IDF

↓

More Important
```

```text
Common Word

↓

Low IDF

↓

Less Important
```

---

# 📊 Understanding IDF with an Example

Suppose we have three documents.

```text
Doc 1

AI is amazing.
```

```text
Doc 2

AI is useful.
```

```text
Doc 3

Machine Learning is powerful.
```

Word appearances:

| Word | Appears In |
|------|-----------:|
| AI | 2 documents |
| Machine | 1 document |
| Learning | 1 document |
| is | 3 documents |
| amazing | 1 document |

Notice:

- **is** appears everywhere → low IDF
- **Machine** appears once → high IDF

Therefore:

```text
Machine

↓

Higher Importance
```

than

```text
is
```

---

# ⚙️ TF-IDF Workflow

```text
Documents

↓

Text Preprocessing

↓

Tokenization

↓

Vocabulary

↓

Calculate TF

↓

Calculate IDF

↓

Multiply TF × IDF

↓

TF-IDF Vector

↓

Machine Learning Model
```

---

# 📝 Simple TF-IDF Example

Suppose we have two documents.

### Document 1

```text
AI AI Machine
```

### Document 2

```text
Machine Learning
```

Vocabulary:

```text
AI

Machine

Learning
```

TF:

| Word | Doc 1 | Doc 2 |
|------|------:|------:|
| AI | 2 | 0 |
| Machine | 1 | 1 |
| Learning | 0 | 1 |

IDF intuition:

- **AI** appears in one document → High IDF
- **Machine** appears in both documents → Lower IDF
- **Learning** appears in one document → High IDF

Final TF-IDF:

- AI → High score in Document 1
- Machine → Lower score
- Learning → High score in Document 2

---

# 📈 Understanding TF-IDF Scores

Generally:

| TF | IDF | Importance |
|---:|----:|------------|
| High | High | ⭐ Very High |
| High | Low | Medium |
| Low | High | Medium |
| Low | Low | Very Low |

A word is considered highly informative when it is common in one document but uncommon across the rest of the corpus.

---

# 🌍 Real-World Example 1 — Search Engine

User searches:

```text
machine learning books
```

TF-IDF identifies important words:

```text
machine

learning

books
```

Words such as:

```text
the

is

and
```

receive much lower weights.

This improves search relevance.

---

# 🌍 Real-World Example 2 — News Classification

Headline:

```text
Earthquake hits Japan.
```

Important words:

```text
earthquake

japan
```

Less important words:

```text
the

in

is
```

TF-IDF highlights the informative terms for the classifier.

---

# 🌍 Real-World Example 3 — Resume Screening

Resume:

```text
Python

Machine Learning

TensorFlow

SQL
```

TF-IDF assigns higher importance to technical skills that distinguish one resume from another.

Recruitment systems can use these weighted features for candidate matching.

---

# 💼 Business Example

## Product Review Analysis

An e-commerce company receives one million customer reviews.

Example review:

```text
This laptop has excellent battery life.
```

Pipeline:

```text
Customer Reviews

↓

Text Preprocessing

↓

Tokenization

↓

TF-IDF

↓

Machine Learning

↓

Positive Review Detection

↓

Business Dashboard
```

### Business Benefits

- Better keyword extraction
- More accurate product categorization
- Improved customer insight
- Better recommendation systems

---

# 📊 Bag of Words vs TF-IDF

| Feature | Bag of Words | TF-IDF |
|----------|--------------|---------|
| Counts words | ✅ Yes | ✅ Yes |
| Uses word importance | ❌ No | ✅ Yes |
| Reduces common word influence | ❌ No | ✅ Yes |
| Better feature representation | ❌ Limited | ✅ Better |
| Commonly used in traditional ML | ✅ Yes | ✅ Yes |

---

# 📊 TF vs IDF

| Term Frequency (TF) | Inverse Document Frequency (IDF) |
|---------------------|----------------------------------|
| Measures frequency inside one document | Measures rarity across all documents |
| High if word appears often | High if word appears in few documents |
| Document-specific | Corpus-specific |

---

# 📊 TF-IDF vs Word Embeddings

| TF-IDF | Word Embeddings |
|---------|-----------------|
| Statistical weighting | Learns semantic meaning |
| Sparse vectors | Dense vectors |
| Does not capture context | Captures semantic relationships |
| Traditional NLP | Modern NLP |

---

# 🌟 Advantages of TF-IDF

- Easy to understand
- Simple to implement
- Highlights important words
- Reduces influence of common words
- Improves traditional Machine Learning models
- Works well for document classification and information retrieval

---

# ⚠️ Limitations of TF-IDF

- Ignores word order
- Ignores grammar
- Does not understand context
- Cannot recognize synonyms
- Cannot capture semantic meaning
- Produces sparse vectors
- Less effective than embeddings and Transformers for many modern NLP tasks

---

# 🎤 Interview Insight

### Question

**What is TF-IDF, and why is it better than Bag of Words?**

### Sample Answer

> TF-IDF stands for Term Frequency–Inverse Document Frequency. It measures the importance of a word by considering both how often it appears in a document and how rare it is across the entire corpus. Unlike Bag of Words, which only counts word occurrences, TF-IDF assigns lower weights to very common words and higher weights to informative words, making it a more useful feature representation for many traditional NLP tasks.

---

# ⚠️ Common Beginner Mistakes

### ❌ Mistake 1

Thinking TF-IDF understands language.

✅ **Correct**

TF-IDF is a statistical weighting technique. It does not understand grammar or meaning.

---

### ❌ Mistake 2

Believing rare words are always important.

✅ **Correct**

Some rare words may simply be spelling mistakes, identifiers, or irrelevant terms. TF-IDF measures rarity, not usefulness.

---

### ❌ Mistake 3

Assuming TF-IDF preserves word order.

✅ **Correct**

Like Bag of Words, TF-IDF ignores the order of words.

---

### ❌ Mistake 4

Thinking TF-IDF has replaced modern NLP models.

✅ **Correct**

Modern NLP often relies on word embeddings and Transformer-based models, but TF-IDF remains valuable for many traditional Machine Learning tasks.

---

# 📝 Key Takeaways

- TF-IDF measures how important a word is within a document relative to a corpus.
- It combines **Term Frequency (TF)** and **Inverse Document Frequency (IDF)**.
- Common words receive lower weights, while informative words receive higher weights.
- TF-IDF is an improvement over Bag of Words because it considers word importance, not just frequency.
- Although modern NLP frequently uses embeddings and Transformers, TF-IDF remains a strong baseline for document classification, search, and information retrieval.

---

# 📖 Vocabulary

| Term | Meaning |
|------|---------|
| TF (Term Frequency) | Frequency of a word within a document |
| IDF (Inverse Document Frequency) | Measure of how rare a word is across a corpus |
| TF-IDF | Product of TF and IDF used to weight word importance |
| Corpus | Collection of documents |
| Vocabulary | Set of unique words across a corpus |
| Feature Vector | Numerical representation of text |
| Sparse Vector | Vector containing many zero values |
| Keyword Extraction | Identifying the most informative words in a document |
| Information Retrieval | Finding relevant documents in response to a query |
| Weight | Numerical value representing a feature's importance |

---

# ❓ Revision Questions

1. What is TF-IDF?
2. Why was TF-IDF developed?
3. What is Term Frequency (TF)?
4. What is Inverse Document Frequency (IDF)?
5. Why do common words receive lower TF-IDF scores?
6. Compare Bag of Words and TF-IDF.
7. What are the advantages of TF-IDF?
8. What are its limitations?
9. Why is TF-IDF useful for search engines?
10. Why have many modern NLP systems moved toward word embeddings and Transformer-based models?

---

# ⏱️ One-Minute Revision

```text
Documents

↓

Text Preprocessing

↓

Tokenization

↓

Vocabulary

↓

Calculate

TF

↓

Calculate

IDF

↓

TF × IDF

↓

Weighted Feature Vector

↓

Machine Learning Model

Key Ideas

✔ Frequent in One Document → Higher TF
✔ Rare Across Corpus → Higher IDF
✔ Common Words → Lower Weight
✔ Informative Words → Higher Weight

Applications

Search Engines

Document Classification

Keyword Extraction

Spam Detection

Resume Screening
```

---

# ➡️ Next Chapter

**08 – Word Embeddings**

> Learn how Word Embeddings represent words as dense numerical vectors that capture semantic meaning, enabling AI models to understand relationships such as *king → queen* and *Paris → France*.