# Social Media Market Sentiment Analysis & NLP Classification Pipeline

**Author:** Ahmed Noureldin  
**Domain:** Natural Language Processing, Market Sentiment Analysis & Text Analytics  
**Dataset:** Sentiment140 Dataset (1,600,000 Sample Records | Balanced Corpus)

---

## 1. Executive Summary & Problem Context

Financial market participants and brand risk officers increasingly rely on high-velocity social stream processing to detect sentiment regime shifts, consumer dissatisfaction spikes, and emerging brand reputation events.

This repository implements a lightweight, high-throughput NLP classification pipeline capable of sub-millisecond per-document inference.

---

## 2. Text Preprocessing & Feature Extraction

- **Text Normalization:** Strips URLs, user mentions (`@user`), emojis/special punctuation, contractions expansion, and lowercase normalization.
- **Sparse Feature Extraction:** Sublinear TF-IDF vectorization with 35,000 vocabulary dimensions spanning unigram and bigram ranges ($N$-grams: 1-2) with min/max document frequency thresholds.

---

## 3. Model Evaluation & Benchmark Comparison

Evaluated across 5-Fold Stratified Cross-Validation:

| Model | ROC-AUC | PR-AUC | F1-Score | Inference Latency |
|---|---|---|---|---|
| **Logistic Regression (L2)** | **0.8614** | **0.8520** | **0.7840** | 0.04 ms/doc |
| **Linear SVM (SGD)** | 0.8540 | 0.8410 | 0.7760 | 0.03 ms/doc |
| **Multinomial Naive Bayes** | 0.8380 | 0.8250 | 0.7610 | **0.01 ms/doc** |

---

## 4. Key Predictive Tokens

- **Top Positive Predictors:** `thanks`, `great`, `awesome`, `love`, `glad`, `good`, `perfect`
- **Top Negative Predictors:** `sad`, `sorry`, `miss`, `hate`, `hurts`, `fail`, `bad`, `worst`

---

## Repository Structure

```
├── Twitter_Sentiment_Notebook.ipynb   # Full preprocessing, TF-IDF vectorization & model evaluation
├── README.md                          # Project documentation
└── README_AR.md                       # Detailed Arabic overview
```
