# 📰 Fake News Detection using Semantic Classification

This project focuses on building a **semantic classification model** to automatically classify news articles as either **fake** or **true**, using **Word2Vec embeddings** and **supervised learning** algorithms. The aim is to address the growing concern around misinformation by leveraging Natural Language Processing (NLP) techniques that go beyond surface-level text analysis.

---

## 🚀 Objective

To develop a text classification system that understands the **semantic meaning** of news articles and accurately detects fake news using **Word2Vec** and supervised machine learning models.

---

## 📊 Business Problem

Fake news can spread misinformation and harm public trust. In an era of digital media overload, identifying fake content is critical. This project aims to:
- Detect fake news with high accuracy.
- Minimize false positives and false negatives.
- Enable trust in automated news validation systems.

---

## 🛠️ Methodology

1. **Data Preparation**
   - Merged true and fake news datasets.
   - Cleaned nulls and duplicates.
   - Labeled data (1 for true, 0 for fake).

2. **Text Preprocessing**
   - Lowercasing
   - Punctuation and stopword removal
   - Lemmatization

3. **Semantic Feature Extraction**
   - Trained or used pre-trained **Word2Vec** model.
   - Averaged word vectors to represent news articles.

4. **Train-Validation Split**
   - 70% training / 30% validation split (stratified).

5. **Model Training**
   - Trained Logistic Regression, Decision Tree, and Random Forest models.

6. **Evaluation**
   - Metrics used: Accuracy, Precision, Recall, F1-Score.
   - Best model selected based on F1-Score.

---

## 🤖 Models & Performance

| Model               | Accuracy | Precision | Recall | F1-Score |
|--------------------|----------|-----------|--------|----------|
| Logistic Regression| 0.9037   | 0.8931    | 0.9065 | 0.8997   |
| Decision Tree      | 0.9037   | 0.8931    | 0.9065 | 0.8997   |
| Random Forest      | 0.9055   | 0.9071    | 0.8932 | **0.9001** |

✅ **Final Model Chosen**: Random Forest  
📌 **Evaluation Metric Prioritized**: F1-Score (for balanced precision and recall)

---

## 🔍 Key Insights

- **True news** typically follows structured and factual language.
- **Fake news** tends to be emotionally charged or semantically inconsistent.
- Word2Vec effectively captured semantic nuances and enhanced classification.
- Random Forest offered the best balance of performance and generalization.

---
