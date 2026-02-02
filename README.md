# 🔎 Hybrid Search Engine (Lexical + Semantic Retrieval)
[![Python](https://img.shields.io/badge/Python-3.x-blue)](#)
[![NLP](https://img.shields.io/badge/NLP-Information%20Retrieval-green)](#)
[![Dataset](https://img.shields.io/badge/Dataset-MS%20MARCO-orange)](#)
[![Model](https://img.shields.io/badge/Retrieval-BM25%20%2B%20Dense-blueviolet)](#)

A **hybrid information retrieval system** that combines **lexical retrieval (BM25)** with **semantic dense retrieval (transformer-based embeddings)** using **weighted score fusion**, evaluated on the **MS MARCO Passage Ranking dataset**.

---

## 📌 Overview

Traditional lexical search methods such as **BM25** excel at exact keyword matching but lack semantic understanding.  
Conversely, dense retrieval models capture semantic similarity but may miss precise lexical signals.

This project explores whether **combining both approaches** through a hybrid fusion framework can improve passage ranking performance and robustness.

---

## 🎯 Project Objectives

- Implement a **BM25-based lexical retrieval system**
- Implement **semantic dense retrieval** using transformer embeddings
- Combine both signals using **weighted score fusion**
- Compare:
  - BM25-only retrieval
  - Dense semantic retrieval
  - Hybrid lexical + semantic retrieval
- Analyze strengths and limitations of each approach

---

## 📊 Dataset

This project uses the **MS MARCO Passage Ranking Dataset**, a standard benchmark in information retrieval research.

🔗 Dataset source:  
https://microsoft.github.io/msmarco/Datasets.html

### Files Used
- `collection.tar.gz` — document passages  
- `queries.train.tsv` — training queries  
- `qrels.train.tsv` — relevance judgments  

Each passage is ranked based on relevance to a given query.

---

## ✨ What This Project Does

- Loads and preprocesses MS MARCO passages and queries
- Builds a **BM25 index** for lexical search
- Generates **dense embeddings** for semantic retrieval
- Computes similarity scores between queries and passages
- Applies **weighted fusion** to combine retrieval signals
- Evaluates ranking effectiveness across retrieval strategies

---

## 🧰 Technology Stack

- **Python**
- **Jupyter Notebook**
- **Information Retrieval (IR)**
- **BM25**
- **Transformer-based embeddings**
- **NumPy, Pandas**
- **Scikit-learn / PyTorch**

