# 🧠 NLP Pipeline with Hugging Face Transformers

This project demonstrates the use of Hugging Face's `transformers` library to perform multiple natural language processing (NLP) tasks using the high-level `pipeline()` API.

## 📋 Overview

The notebook `pipeline models.ipynb` contains implementations of several popular NLP tasks. All tasks use pre-trained deep learning models, made accessible through simple function calls. The following tasks are included:

---

## ✅ Implemented NLP Tasks

### 1. Question Answering
A question is asked based on a given context. The model extracts the most relevant answer span from the context.

---

### 2. Text Summarization
A long paragraph of dummy text is passed to the model, and a shorter summary is generated automatically using transformer-based summarization.

---

### 3. Sentiment Analysis
A sentence is classified into positive or negative sentiment using a pre-trained classifier.

---

### 4. Named Entity Recognition (NER)
The model identifies entities such as people, places, and organizations in a given sentence.

---

### 5. Translation (English to French)
A simple English sentence is translated to French using a pre-trained translation model.

---

### 6. Zero-Shot Classification
The model classifies a sentence into user-defined categories, even if it was not specifically trained on them.

---

## 🧰 Requirements

To run this notebook, install the following:

```bash
pip install transformers
pip install torch
