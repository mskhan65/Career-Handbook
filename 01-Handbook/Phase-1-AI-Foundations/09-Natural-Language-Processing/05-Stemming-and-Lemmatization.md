# 🌱 Stemming and Lemmatization

**Difficulty:** ⭐ Beginner  
**Estimated Reading Time:** 30–35 minutes  
**Prerequisites:** 01 – Introduction to NLP, 02 – What is NLP?, 03 – Text Preprocessing, 04 – Tokenization  
**Last Updated:** July 2026

---

# 📖 Introduction

Humans naturally understand that words like:

- play
- playing
- played
- plays

all refer to the same basic concept.

However, computers initially treat each of these as different words.

This creates a larger vocabulary, increases computational complexity, and makes learning more difficult.

To solve this problem, NLP uses two important preprocessing techniques:

- **Stemming**
- **Lemmatization**

Both techniques reduce different forms of a word to a common representation, making text analysis more efficient.

---

# 🎯 Learning Goals

After completing this chapter, you will be able to:

- Understand why stemming and lemmatization are important.
- Learn how stemming works.
- Learn how lemmatization works.
- Compare stemming and lemmatization.
- Identify when each technique should be used.
- Explore real-world applications.

---

# 🤔 Why Do We Need Stemming and Lemmatization?

Consider these sentences:

```text
He plays football.

She is playing football.

They played football yesterday.
```

Without preprocessing, the computer sees:

```text
plays

playing

played
```

as three different words.

However, they all represent the same action.

Reducing them to a common base form helps NLP models recognize that they are related.

---

# 🌱 What is Stemming?

**Stemming** is the process of reducing a word to its **stem** by removing prefixes or suffixes.

The resulting stem may **not** always be a valid English word.

Example:

| Original Word | Stem |
|--------------|------|
| playing | play |
| played | play |
| player | player |
| studies | studi |
| studying | studi |
| running | run |

Notice:

```text
studies

↓

studi
```

"studi" is **not** a real English word.

It is simply the stem produced by the stemming algorithm.

---

# ⚙️ How Stemming Works

A stemming algorithm removes common endings.

Example:

```text
playing

↓

Remove "ing"

↓

play
```

Another example:

```text
worked

↓

Remove "ed"

↓

work
```

The algorithm applies predefined rules without understanding grammar or context.

---

# 🌿 What is Lemmatization?

**Lemmatization** reduces a word to its **lemma**, which is the correct dictionary form of the word.

Unlike stemming, the output is a meaningful word.

Example:

| Original Word | Lemma |
|--------------|-------|
| playing | play |
| played | play |
| better | good |
| studies | study |
| running | run |
| mice | mouse |

Notice:

```text
better

↓

good
```

This transformation is based on language rules rather than simply removing characters.

---

# ⚙️ How Lemmatization Works

Lemmatization considers:

- Grammar
- Context
- Part of Speech (POS)
- Dictionary lookups

Example:

```text
running

↓

Verb

↓

run
```

Another example:

```text
better

↓

Adjective

↓

good
```

Because of this, lemmatization is generally more accurate than stemming.

---

# 📊 Stemming vs Lemmatization

| Feature | Stemming | Lemmatization |
|----------|-----------|---------------|
| Output | Stem | Dictionary word (lemma) |
| Uses grammar | ❌ No | ✅ Yes |
| Uses dictionary | ❌ No | ✅ Yes |
| Speed | Faster | Slower |
| Accuracy | Lower | Higher |
| Produces real words | Not always | Yes |

---

# 🧩 Examples

## Example 1

Original:

```text
playing
```

Stemming:

```text
play
```

Lemmatization:

```text
play
```

---

## Example 2

Original:

```text
studies
```

Stemming:

```text
studi
```

Lemmatization:

```text
study
```

---

## Example 3

Original:

```text
better
```

Stemming:

```text
better
```

Lemmatization:

```text
good
```

---

## Example 4

Original:

```text
mice
```

Stemming:

```text
mice
```

Lemmatization:

```text
mouse
```

---

# 🔄 Stemming Workflow

```text
Original Word

↓

Remove Prefixes/Suffixes

↓

Stem

↓

NLP Model
```

Example:

```text
playing

↓

play
```

---

# 🔄 Lemmatization Workflow

```text
Original Word

↓

Grammar Analysis

↓

Dictionary Lookup

↓

Lemma

↓

NLP Model
```

Example:

```text
playing

↓

Verb

↓

play
```

---

# 🌍 Real-World Example 1 — Search Engine

A user searches:

```text
running shoes
```

Another user searches:

```text
run shoes
```

After lemmatization:

```text
running

↓

run
```

Both searches are treated similarly, improving search results.

---

# 🌍 Real-World Example 2 — Customer Review Analysis

Reviews:

```text
I liked the product.

I like the product.

I am liking the product.
```

After preprocessing:

```text
like

like

like
```

The sentiment analysis model now recognizes that all three reviews express the same basic action.

---

# 🌍 Real-World Example 3 — Document Search

Documents contain:

```text
connect

connected

connecting

connection
```

After preprocessing, related terms become easier to group, improving document retrieval.

---

# 💼 Business Example

## E-Commerce Product Search

Customers search for:

```text
running shoes

runner shoes

run shoes
```

Pipeline:

```text
Customer Query

↓

Tokenization

↓

Lemmatization

↓

Search Index

↓

Relevant Products
```

### Business Benefits

- Better search accuracy
- Improved customer experience
- Higher conversion rates
- More relevant recommendations

---

# 📊 Advantages of Stemming

- Very fast
- Simple implementation
- Reduces vocabulary size
- Suitable for large datasets
- Lower computational cost

---

# ⚠️ Limitations of Stemming

- Can produce non-dictionary words
- Ignores grammar
- Less accurate
- May incorrectly merge unrelated words
- Can remove too many characters (over-stemming)

---

# 📊 Advantages of Lemmatization

- Produces meaningful words
- Uses grammar and context
- Higher accuracy
- Better language understanding
- Preferred for modern NLP applications

---

# ⚠️ Limitations of Lemmatization

- Slower than stemming
- Requires linguistic resources
- More computationally expensive
- More complex to implement

---

# 📊 Stemming vs Lemmatization vs No Reduction

| Original | No Reduction | Stemming | Lemmatization |
|-----------|--------------|-----------|---------------|
| playing | playing | play | play |
| studies | studies | studi | study |
| running | running | run | run |
| better | better | better | good |
| mice | mice | mice | mouse |

---

# 🌟 When Should You Use Each?

| Situation | Recommended Technique |
|-----------|------------------------|
| Fast preprocessing | Stemming |
| Search engines | Lemmatization |
| Chatbots | Lemmatization |
| Machine Translation | Lemmatization |
| Question Answering | Lemmatization |
| Large-scale indexing | Stemming or Lemmatization, depending on accuracy needs |

In many modern Deep Learning applications, especially those based on Transformers, explicit stemming or lemmatization may be unnecessary because the models often learn relationships between word forms during training.

---

# 🎤 Interview Insight

### Question

**What is the difference between stemming and lemmatization?**

### Sample Answer

> Stemming reduces words to their stems by removing prefixes or suffixes using simple rules. The resulting stem may not be a valid word. Lemmatization reduces words to their dictionary form, called the lemma, by using grammar and vocabulary knowledge. Lemmatization is generally more accurate but computationally more expensive than stemming.

---

# ⚠️ Common Beginner Mistakes

### ❌ Mistake 1

Thinking stemming always produces valid English words.

✅ **Correct**

Stemming often produces stems that are not dictionary words.

---

### ❌ Mistake 2

Believing stemming understands grammar.

✅ **Correct**

Stemming applies simple rules and does not consider grammatical context.

---

### ❌ Mistake 3

Assuming lemmatization is always necessary.

✅ **Correct**

Some modern NLP models, particularly Transformer-based models, can perform well without explicit stemming or lemmatization.

---

### ❌ Mistake 4

Thinking stemming and lemmatization produce identical results.

✅ **Correct**

Lemmatization generally produces linguistically correct words, while stemming focuses on reducing words quickly using heuristic rules.

---

# 📝 Key Takeaways

- Stemming and lemmatization reduce different forms of words to a common representation.
- Stemming is faster but may produce non-dictionary words.
- Lemmatization uses grammar and dictionaries to produce meaningful base forms.
- Lemmatization is generally more accurate but computationally more expensive.
- The choice between stemming and lemmatization depends on the NLP task, performance requirements, and model architecture.

---

# 📖 Vocabulary

| Term | Meaning |
|------|---------|
| Stem | A reduced form of a word produced by stemming |
| Stemming | Removing prefixes or suffixes to obtain a stem |
| Lemma | The dictionary form of a word |
| Lemmatization | Reducing a word to its lemma using grammar and vocabulary |
| Vocabulary | Collection of unique words or tokens in a dataset |
| Part of Speech (POS) | Grammatical category such as noun, verb, or adjective |
| Dictionary Lookup | Finding the standard form of a word using a lexical resource |
| Over-stemming | Reducing words too aggressively, causing unrelated words to appear similar |
| Under-stemming | Failing to reduce related words to the same base form |
| Linguistic Resource | A language resource, such as a dictionary or lexical database, used in NLP |

---

# ❓ Revision Questions

1. What is stemming?
2. What is lemmatization?
3. Why are stemming and lemmatization useful in NLP?
4. What is the difference between a stem and a lemma?
5. Why can stemming produce non-dictionary words?
6. Why is lemmatization generally more accurate?
7. Compare stemming and lemmatization in terms of speed and accuracy.
8. When might stemming be preferred over lemmatization?
9. How can lemmatization improve search engines?
10. Why do many modern Transformer-based models not require explicit stemming or lemmatization?

---

# ⏱️ One-Minute Revision

```text
Words

↓

playing

played

plays

↓

Word Reduction

├── Stemming
│     ↓
│   Remove Prefixes/Suffixes
│     ↓
│   Stem
│
└── Lemmatization
      ↓
Grammar + Dictionary
      ↓
Lemma

↓

Benefits

✔ Smaller Vocabulary
✔ Better Text Consistency
✔ Improved Search
✔ Better NLP Performance

↓

Comparison

Stemming

✔ Faster
✔ Simpler
✘ Less Accurate

Lemmatization

✔ More Accurate
✔ Dictionary Words
✘ Slower
```

---

# ➡️ Next Chapter

**06 – Bag of Words (BoW)**

> Learn how text is converted into numerical features using the Bag of Words model, one of the earliest and most important techniques for representing text in Machine Learning.