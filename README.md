# 🚀 Question Answering System using BERT

This project implements an extractive Question Answering (QA) system using a pretrained BERT model fine-tuned on a QA dataset.

The model learns to extract answer spans directly from context passages given a question.

---

## 📌 Project Overview

This project fine-tunes a transformer-based model (`bert-base-uncased`) for extractive question answering.

Given:
- A context paragraph
- A question

The model predicts:
- Start position of the answer
- End position of the answer

---

## 🏗️ Pipeline Architecture

1. Load QA dataset
2. Tokenize question and context pairs
3. Handle long contexts with truncation & stride
4. Map answer spans to token positions
5. Fine-tune BERT for span prediction
6. Evaluate model performance
7. Run inference on custom examples

---

## 🧠 Technical Concepts Implemented

- Transformer-based extractive QA
- Token position alignment
- Handling offset mappings
- Trainer API (Hugging Face)
- Dynamic padding with DataCollator
- Fine-tuning on GPU (Google Colab)

---

## 🛠️ Tech Stack

- Python
- PyTorch
- Hugging Face Transformers
- Datasets
- Google Colab

---

## 📊 Model

Pretrained model used:
- `bert-base-uncased`

Task:
- Extractive Question Answering

---

## ▶️ How to Run

1. Open the notebook in Google Colab.
2. Install dependencies:
```
!pip install transformers datasets accelerate -q
```
3. Run all cells sequentially.

---

## 🧪 Example

**Context:**
"Machine learning is a subset of artificial intelligence that focuses on learning from data."

**Question:**
"What is machine learning a subset of?"

**Predicted Answer:**
"artificial intelligence"

---

## 🔗 Open in Colab
https://colab.research.google.com/drive/1oiYpyBYwxsqDIj0xLCtxT1Ein_LUC7LX?usp=sharing
