# 🧠 Word Embeddings

**Difficulty:** ⭐⭐ Beginner to Intermediate  
**Estimated Reading Time:** 40–45 minutes  
**Prerequisites:** 01 – Introduction to NLP, 02 – What is NLP?, 03 – Text Preprocessing, 04 – Tokenization, 05 – Stemming and Lemmatization, 06 – Bag of Words, 07 – TF-IDF  
**Last Updated:** July 2026

---

# 📖 Introduction

In the previous chapters, you learned two popular text representation techniques:

- Bag of Words (BoW)
- TF-IDF

Although these methods convert text into numbers, they have a major limitation:

> **They do not understand the meaning of words.**

For example:

```text
King

Queen

Man

Woman
```

To a Bag of Words model, these are simply different words with different counts.

However, humans know that:

- King and Queen are related.
- Man and Woman are related.
- King is closer in meaning to Queen than to Apple.

Modern AI systems learn these relationships using **Word Embeddings**.

Word Embeddings represent words as dense numerical vectors where **similar words have similar vector representations**.

This breakthrough made NLP much more powerful and paved the way for Deep Learning and Large Language Models (LLMs).

---

# 🎯 Learning Goals

After completing this chapter, you will be able to:

- Understand what Word Embeddings are.
- Learn why embeddings are better than BoW and TF-IDF.
- Understand dense vector representations.
- Explore semantic relationships between words.
- Learn popular embedding techniques.
- Understand real-world applications.

---

# 🤔 Why Do We Need Word Embeddings?

Consider the following words:

```text
Car

Automobile
```

Humans know these words have nearly the same meaning.

Bag of Words:

```text
Car

↓

Word #18
```

```text
Automobile

↓

Word #42
```

The model sees them as unrelated.

Word Embeddings place them close together in a mathematical space because they appear in similar contexts.

---

# 📖 What are Word Embeddings?

**Word Embeddings** are dense numerical vector representations of words that capture their meanings and relationships.

Instead of representing words as simple counts, embeddings represent each word as a list of numerical values.

Example:

```text
King

↓

[0.82, -0.14, 0.67, ...]
```

```text
Queen

↓

[0.79, -0.18, 0.65, ...]
```

The actual vectors may contain dozens, hundreds, or even thousands of dimensions depending on the model.

Words with similar meanings tend to have similar vectors.

---

# ⚙️ From Words to Vectors

Traditional NLP:

```text
Word

↓

Integer ID

↓

Model
```

Modern NLP:

```text
Word

↓

Embedding Vector

↓

Neural Network

↓

Prediction
```

The embedding vector carries much richer information than a simple integer ID.

---

# 🧩 Dense vs Sparse Vectors

## Sparse Vector

Bag of Words:

```text
Vocabulary

↓

[0, 0, 1, 0, 0, 0, 1, 0, ...]
```

Characteristics:

- Mostly zeros
- Very large
- No semantic meaning

---

## Dense Vector

Word Embedding:

```text
[0.42, -0.15, 0.87, 0.31, ...]
```

Characteristics:

- Small
- Dense
- Contains semantic information
- Learned automatically

---

# 📊 Sparse vs Dense Representations

| Feature | Sparse (BoW / TF-IDF) | Dense (Embeddings) |
|----------|------------------------|--------------------|
| Mostly zeros | ✅ Yes | ❌ No |
| Compact | ❌ No | ✅ Yes |
| Captures meaning | ❌ No | ✅ Yes |
| Learns relationships | ❌ No | ✅ Yes |
| Used in modern Deep Learning | ❌ Rarely | ✅ Yes |

---

# 🧠 How Word Embeddings Learn Meaning

Instead of memorizing definitions, embedding models learn from context.

Example:

```text
The cat drinks milk.

↓

Cat appears near milk.
```

```text
The dog drinks water.

↓

Dog appears near water.
```

Over millions or billions of sentences, the model learns which words frequently appear together.

This idea is often summarized as:

> **Words that appear in similar contexts tend to have similar meanings.**

---

# 🌍 Semantic Relationships

One of the most impressive properties of embeddings is that they capture semantic relationships.

Example:

```text
King

↓

Close to

↓

Queen
```

Another example:

```text
Doctor

↓

Close to

↓

Nurse
```

Another:

```text
Paris

↓

Close to

↓

France
```

Words with related meanings are located near one another in the embedding space.

---

# 🎨 Visualizing Word Embeddings

Imagine a map where each point represents a word.

```text
                Queen

                  ●

         Princess     King

             ●          ●

Woman ●                  ● Man

             ●

          Girl

                 ● Boy
```

Nearby words tend to have similar meanings or roles.

In reality, embeddings exist in many dimensions, but they can be visualized in two or three dimensions for understanding.

---

# 📈 Famous Embedding Example

One well-known example demonstrates how vector arithmetic can capture relationships.

```text
King

− Man

+ Woman

↓

Queen
```

This illustrates that embedding vectors can encode meaningful linguistic relationships.

While the exact result depends on the embedding model, it shows how semantic patterns can emerge from training.

---

# ⚙️ How Word Embeddings are Learned

Training data:

```text
Millions of Sentences

↓

Tokenization

↓

Neural Network

↓

Predict Context Words

↓

Update Embedding Vectors

↓

Learn Word Meanings
```

During training:

- Similar words move closer together.
- Unrelated words move farther apart.
- Relationships gradually emerge.

---

# 🏗️ Popular Word Embedding Models

Several models have been developed to learn word embeddings.

### Word2Vec

Developed by Google.

Two main training approaches:

- Continuous Bag of Words (CBOW)
- Skip-Gram

Word2Vec learns embeddings by predicting surrounding words.

---

### GloVe (Global Vectors)

Developed by Stanford University.

Instead of focusing only on nearby words, GloVe also uses global word co-occurrence statistics from the entire corpus.

---

### FastText

Developed by Meta (formerly Facebook).

Unlike Word2Vec, FastText represents words using **subword information**.

Example:

```text
playing

↓

play

ing
```

This allows FastText to better handle rare and unseen words.

---

### Contextual Embeddings

Modern Transformer models generate **contextual embeddings**.

The meaning of a word depends on its sentence.

Example:

```text
I sat on the bank.
```

versus

```text
I deposited money in the bank.
```

The word **bank** receives different embeddings because its meaning changes with context.

Models such as **BERT** and **GPT** use contextual embeddings.

---

# 🌍 Real-World Example 1 — Search Engine

User searches:

```text
car
```

Documents contain:

```text
automobile
```

Traditional search might miss the match.

Embedding-based search recognizes that:

```text
car

≈

automobile
```

This improves search quality.

---

# 🌍 Real-World Example 2 — Recommendation Systems

An online bookstore analyzes descriptions of books.

Books with similar topics receive similar embedding vectors.

Recommendations become more relevant because the system compares meanings rather than exact words.

---

# 🌍 Real-World Example 3 — Chatbots

User asks:

```text
How do I reset my password?
```

Another user asks:

```text
I forgot my password.
```

Although the wording is different, embeddings help the chatbot recognize that both requests express a similar intent.

---

# 💼 Business Example

## Intelligent Customer Support

A bank receives thousands of customer questions every day.

Customers may ask:

```text
How do I transfer money?
```

```text
How can I send funds?
```

```text
How do I make a payment?
```

Embedding-based NLP recognizes that these questions are closely related.

Pipeline:

```text
Customer Question

↓

Tokenization

↓

Word Embeddings

↓

Intent Detection

↓

Answer Retrieval

↓

Customer Response
```

### Business Benefits

- Better chatbot accuracy
- Improved search
- Faster customer support
- Better multilingual understanding
- Higher customer satisfaction

---

# 📊 Bag of Words vs TF-IDF vs Word Embeddings

| Feature | Bag of Words | TF-IDF | Word Embeddings |
|----------|--------------|---------|-----------------|
| Word counts | ✅ Yes | ✅ Yes | ❌ No |
| Word importance | ❌ No | ✅ Yes | Learns implicitly |
| Captures meaning | ❌ No | ❌ No | ✅ Yes |
| Understands similarity | ❌ No | ❌ No | ✅ Yes |
| Dense vectors | ❌ No | ❌ No | ✅ Yes |
| Used in modern LLMs | ❌ No | ❌ No | ✅ Yes |

---

# 📊 Static vs Contextual Embeddings

| Static Embeddings | Contextual Embeddings |
|-------------------|-----------------------|
| One vector per word | Different vector depending on context |
| Word2Vec | BERT |
| GloVe | GPT |
| FastText | Modern Transformers |
| Simpler | More powerful |

---

# 🌟 Advantages of Word Embeddings

- Capture semantic meaning
- Learn relationships between words
- Dense numerical vectors
- Better than BoW and TF-IDF for many tasks
- Improve Machine Learning and Deep Learning performance
- Handle synonyms more effectively
- Enable semantic search and recommendation systems

---

# ⚠️ Limitations of Word Embeddings

- Require large amounts of training data
- More computationally expensive than BoW
- Static embeddings cannot distinguish different meanings of the same word
- May learn biases present in training data
- High-quality embeddings require significant computational resources

---

# 🎤 Interview Insight

### Question

**What are Word Embeddings, and why are they better than Bag of Words?**

### Sample Answer

> Word Embeddings are dense numerical vector representations of words that capture semantic meaning and relationships. Unlike Bag of Words, which only counts word occurrences, embeddings place similar words close together in vector space. This allows NLP models to recognize synonyms, semantic similarity, and contextual relationships, making embeddings much more effective for modern Machine Learning and Deep Learning applications.

---

# ⚠️ Common Beginner Mistakes

### ❌ Mistake 1

Thinking embeddings are just word counts.

✅ **Correct**

Embeddings represent semantic meaning, not frequencies.

---

### ❌ Mistake 2

Believing similar spellings always produce similar embeddings.

✅ **Correct**

Embeddings are learned from usage and context, not spelling alone.

---

### ❌ Mistake 3

Assuming every embedding model produces identical vectors.

✅ **Correct**

Different models, datasets, and training methods produce different embedding spaces.

---

### ❌ Mistake 4

Thinking static embeddings understand context.

✅ **Correct**

Static embeddings assign one vector per word, while contextual embeddings generate different vectors depending on the surrounding text.

---

# 📝 Key Takeaways

- Word Embeddings represent words as dense numerical vectors.
- Similar words have similar vector representations.
- Embeddings capture semantic relationships that BoW and TF-IDF cannot.
- Popular embedding models include Word2Vec, GloVe, and FastText.
- Modern Transformer-based models such as BERT and GPT generate contextual embeddings that change depending on the sentence.

---

# 📖 Vocabulary

| Term | Meaning |
|------|---------|
| Word Embedding | Dense numerical representation of a word |
| Dense Vector | A compact vector containing mostly non-zero values |
| Sparse Vector | A vector containing many zero values |
| Semantic Similarity | Degree to which words have similar meanings |
| Context | Surrounding words that influence meaning |
| Word2Vec | Neural network model for learning word embeddings |
| GloVe | Embedding model based on global word co-occurrence statistics |
| FastText | Embedding model that uses subword information |
| Static Embedding | One fixed vector for each word |
| Contextual Embedding | A vector whose values depend on the surrounding context |

---

# ❓ Revision Questions

1. What are Word Embeddings?
2. Why are Word Embeddings better than Bag of Words?
3. What is the difference between sparse and dense vectors?
4. How do embeddings learn semantic relationships?
5. What is semantic similarity?
6. Compare Word2Vec, GloVe, and FastText.
7. What are contextual embeddings?
8. Why are contextual embeddings useful for words with multiple meanings?
9. What are the advantages of Word Embeddings?
10. What are the limitations of static embeddings?

---

# ⏱️ One-Minute Revision

```text
Raw Text

↓

Tokenization

↓

Word Embeddings

↓

Dense Vectors

↓

Neural Network

↓

Prediction

Embedding Models

├── Word2Vec
├── GloVe
├── FastText
└── Contextual Embeddings (BERT, GPT)

Key Benefits

✔ Capture Meaning
✔ Learn Similarity
✔ Dense Representation
✔ Better than BoW
✔ Better than TF-IDF

Applications

Semantic Search

Recommendation Systems

Chatbots

Machine Translation

Question Answering

Large Language Models
```

---

# ➡️ Next Chapter

**09 – RNNs for NLP**

> Learn how Recurrent Neural Networks (RNNs) process sequential text data, why they were a major breakthrough for NLP, their limitations, and how they paved the way for LSTMs, GRUs, and modern Transformer architectures.