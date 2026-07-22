# 🔤 Tokenization

**Difficulty:** ⭐ Beginner  
**Estimated Reading Time:** 30–35 minutes  
**Prerequisites:** 01 – Introduction to NLP, 02 – What is NLP?, 03 – Text Preprocessing  
**Last Updated:** July 2026

---

# 📖 Introduction

Imagine you are reading a book.

You naturally recognize:

- Sentences
- Words
- Punctuation
- Paragraphs

However, computers cannot automatically separate text into meaningful units.

For a computer, the sentence:

```text
I love Artificial Intelligence.
```

is simply a sequence of characters.

Before AI models can understand text, the text must first be broken into smaller pieces.

This process is called **Tokenization**.

Tokenization is one of the most important steps in Natural Language Processing because nearly every NLP system begins by converting text into tokens.

---

# 🎯 Learning Goals

After completing this chapter, you will be able to:

- Understand what tokenization is.
- Learn why tokenization is important.
- Explore different types of tokenization.
- Understand how modern NLP models tokenize text.
- Compare word, sentence, character, and subword tokenization.
- Recognize real-world applications of tokenization.

---

# 🤔 What is Tokenization?

**Tokenization** is the process of breaking text into smaller meaningful units called **tokens**.

A token can be:

- A sentence
- A word
- A character
- A subword
- A punctuation symbol (depending on the tokenizer)

Example:

```text
I love NLP.
```

↓

Tokens

```text
["I", "love", "NLP", "."]
```

Each token becomes an individual unit that the NLP model can process.

---

# 🎯 Why is Tokenization Important?

Computers cannot directly understand long strings of text.

Instead, they process text token by token.

Without tokenization:

```text
I love Artificial Intelligence.
```

would be treated as one long string.

With tokenization:

```text
["I"]

["love"]

["Artificial"]

["Intelligence"]
```

The model can analyze each token separately while also learning relationships between them.

---

# ⚙️ Tokenization Workflow

```text
Raw Text

↓

Text Preprocessing

↓

Tokenization

↓

Tokens

↓

Numerical Representation

↓

Machine Learning / Deep Learning Model
```

Tokenization is the bridge between human language and machine-readable data.

---

# 📝 What is a Token?

A **token** is the basic unit of text produced during tokenization.

Examples:

Sentence:

```text
AI is changing the world.
```

Word tokens:

```text
AI

is

changing

the

world
```

Each of these words is considered a token.

---

# 🔠 Types of Tokenization

The most common tokenization methods are:

```text
Tokenization

│

├── Sentence Tokenization

├── Word Tokenization

├── Character Tokenization

└── Subword Tokenization
```

---

# 1️⃣ Sentence Tokenization

Sentence tokenization splits text into individual sentences.

Example:

```text
I love AI.

Machine Learning is exciting.

NLP is fascinating.
```

↓

```text
Sentence 1

Sentence 2

Sentence 3
```

Applications:

- Document summarization
- Question answering
- Translation
- Paragraph analysis

---

# 2️⃣ Word Tokenization

Word tokenization splits sentences into individual words.

Example:

```text
Artificial Intelligence is amazing.
```

↓

```text
Artificial

Intelligence

is

amazing
```

This is the most commonly used tokenization technique in traditional NLP.

---

# 3️⃣ Character Tokenization

Character tokenization splits text into individual characters.

Example:

```text
AI
```

↓

```text
A

I
```

Another example:

```text
Chat
```

↓

```text
C

h

a

t
```

Advantages:

- Very small vocabulary
- Handles unknown words naturally

Disadvantages:

- Longer sequences
- More difficult for models to learn word-level meaning

---

# 4️⃣ Subword Tokenization

Modern NLP models often split words into smaller meaningful pieces.

Example:

```text
unbelievable
```

↓

```text
un

believ

able
```

Another example:

```text
playing
```

↓

```text
play

ing
```

Subword tokenization helps models understand words they have never seen before.

It is widely used in modern Transformer models.

---

# 📊 Comparison of Tokenization Types

| Type | Splits Into | Example |
|------|-------------|---------|
| Sentence | Sentences | "Hello." → One sentence |
| Word | Words | "I love AI" → I, love, AI |
| Character | Characters | "AI" → A, I |
| Subword | Word pieces | "playing" → play, ing |

---

# 🌍 Why Modern AI Uses Subword Tokenization

Languages contain millions of possible words.

Instead of storing every word, modern AI models learn smaller word pieces.

Example:

Known subwords:

```text
play

er

ing

ed
```

Unknown word:

```text
player
```

↓

Split into:

```text
play

er
```

Even if **player** never appeared during training, the model can still understand it using known subwords.

Benefits:

- Smaller vocabulary
- Better handling of rare words
- Better multilingual support
- Improved efficiency

---

# 🔢 Tokens Become Numbers

Computers do not understand words directly.

After tokenization, each token is converted into a numerical ID.

Example:

```text
Sentence

↓

I love NLP
```

↓

Tokens

```text
I

love

NLP
```

↓

Token IDs

```text
101

582

901
```

The actual numbers depend on the tokenizer and vocabulary used by the model.

These token IDs are then converted into vector representations before being processed by neural networks.

---

# 🌍 Real-World Example 1 — ChatGPT

When you ask:

```text
Explain Machine Learning.
```

The model first performs:

```text
Sentence

↓

Subword Tokenization

↓

Token IDs

↓

Transformer Model

↓

Generated Response
```

Without tokenization, the model would not be able to process your prompt.

---

# 🌍 Real-World Example 2 — Machine Translation

Input:

```text
Good morning.
```

↓

Word tokens

↓

Translation model

↓

```text
Buenos días.
```

Tokenization allows the translation model to process the sentence piece by piece.

---

# 🌍 Real-World Example 3 — Sentiment Analysis

Customer review:

```text
I absolutely love this product!
```

↓

Tokens

↓

Sentiment model

↓

Positive

Breaking the sentence into tokens helps the model identify words that express opinion.

---

# 💼 Business Example

## Customer Support Automation

A telecommunications company receives thousands of customer messages each hour.

Message:

```text
My internet connection is very slow today.
```

Pipeline:

```text
Customer Message

↓

Text Preprocessing

↓

Tokenization

↓

Intent Detection

↓

Response Generation
```

Business Benefits:

- Faster support
- Improved customer experience
- Reduced workload
- Better automation

---

# 📊 Word Tokenization vs Character Tokenization

| Word Tokenization | Character Tokenization |
|-------------------|------------------------|
| Splits into words | Splits into individual characters |
| Shorter sequences | Longer sequences |
| Easier semantic understanding | Better for unknown words |
| Larger vocabulary | Smaller vocabulary |

---

# 📊 Word Tokenization vs Subword Tokenization

| Word Tokenization | Subword Tokenization |
|-------------------|----------------------|
| Entire words | Word pieces |
| Struggles with unseen words | Handles unseen words well |
| Larger vocabulary | Smaller vocabulary |
| Traditional NLP | Modern LLMs and Transformers |

---

# 📊 Traditional NLP vs Modern NLP

| Traditional NLP | Modern NLP |
|-----------------|------------|
| Mostly word tokenization | Mostly subword tokenization |
| Fixed vocabulary | Flexible vocabulary |
| Poor handling of unknown words | Better handling of rare and new words |
| Simpler models | Transformer-based models |

---

# 🎤 Interview Insight

### Question

**What is Tokenization, and why is it important?**

### Sample Answer

> Tokenization is the process of splitting text into smaller units called tokens, such as sentences, words, characters, or subwords. It is a fundamental step in NLP because computers cannot directly understand raw text. Tokenization converts language into manageable units that can later be transformed into numerical representations for Machine Learning and Deep Learning models.

---

# ⚠️ Common Beginner Mistakes

### ❌ Mistake 1

Thinking tokens are always complete words.

✅ **Correct**

Modern NLP models often use **subword tokens**, not just full words.

---

### ❌ Mistake 2

Believing every NLP model uses the same tokenizer.

✅ **Correct**

Different models use different tokenization algorithms and vocabularies.

---

### ❌ Mistake 3

Assuming tokenization alone gives meaning to text.

✅ **Correct**

Tokenization only splits text into units. Understanding meaning requires additional processing by Machine Learning or Deep Learning models.

---

### ❌ Mistake 4

Thinking token IDs have universal meanings.

✅ **Correct**

Token IDs are specific to a model's tokenizer and vocabulary. The same word may have different IDs in different models.

---

# 📝 Key Takeaways

- Tokenization breaks text into smaller units called tokens.
- Tokens can represent sentences, words, characters, or subwords.
- Tokenization is a foundational step in every NLP pipeline.
- Modern Transformer models typically use subword tokenization because it handles rare and unseen words efficiently.
- After tokenization, tokens are converted into numerical IDs so AI models can process them.

---

# 📖 Vocabulary

| Term | Meaning |
|------|---------|
| Token | A basic unit of text produced during tokenization |
| Tokenization | Splitting text into smaller units |
| Sentence Tokenization | Splitting text into sentences |
| Word Tokenization | Splitting text into individual words |
| Character Tokenization | Splitting text into individual characters |
| Subword Tokenization | Splitting words into smaller meaningful pieces |
| Vocabulary | The collection of tokens known by a tokenizer or model |
| Token ID | A numerical identifier assigned to a token |
| Unknown Word (OOV) | A word not present in a model's vocabulary |
| Transformer | A Deep Learning architecture that commonly uses subword tokenization |

---

# ❓ Revision Questions

1. What is tokenization?
2. Why is tokenization important in NLP?
3. What is a token?
4. What is the difference between sentence and word tokenization?
5. When is character tokenization useful?
6. Why do modern LLMs prefer subword tokenization?
7. What happens after tokenization?
8. What is a token ID?
9. Compare word tokenization and subword tokenization.
10. Why can different NLP models assign different token IDs to the same word?

---

# ⏱️ One-Minute Revision

```text
Raw Text

↓

Text Preprocessing

↓

Tokenization

↓

Types

├── Sentence
├── Word
├── Character
└── Subword

↓

Tokens

↓

Token IDs

↓

Vector Representation

↓

Machine Learning / Deep Learning Model

↓

Prediction or Response

↓

Modern LLMs

✔ Prefer Subword Tokenization
✔ Handle Rare Words Better
✔ Use Smaller Vocabularies
✔ Improve Efficiency
```

---

# ➡️ Next Chapter

**05 – Stemming and Lemmatization**

> Learn how NLP reduces words to their root or base forms using stemming and lemmatization, improving consistency and helping models treat related word forms as the same concept.