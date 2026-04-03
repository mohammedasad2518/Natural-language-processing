# 🚀 BERT IMDb Sentiment Analysis

## 📌 Project Overview

This project demonstrates fine-tuning a BERT (Bidirectional Encoder Representations from Transformers) model on the IMDb dataset for binary sentiment classification (positive vs negative reviews).

The goal is to build a robust NLP pipeline capable of understanding and classifying movie reviews with high accuracy.

---

## 🧠 Key Highlights

- Fine-tuned BERT (bert-base-uncased) using Hugging Face Transformers
- Used IMDb dataset (25,000 training + 25,000 testing samples)
- Achieved ~92% accuracy on test data
- Implemented full NLP pipeline:
  - Data loading
  - Text preprocessing
  - Tokenization
  - Model training
  - Evaluation

---

## ⚙️ Technologies Used

- Python 🐍
- PyTorch 🔥
- Hugging Face Transformers 🤗
- Datasets Library
- Scikit-learn
- Matplotlib & Seaborn

---

## 🔄 Workflow

1️⃣ Data Loading

Dataset is loaded using Hugging Face:

from datasets import load_dataset
dataset = load_dataset("imdb")

---

2️⃣ Preprocessing

- Lowercasing text
- Cleaning input data

---

3️⃣ Tokenization

Using BERT tokenizer:

from transformers import BertTokenizer
tokenizer = BertTokenizer.from_pretrained("bert-base-uncased")

---

4️⃣ Model Training

Fine-tuned BERT model:

from transformers import BertForSequenceClassification
model = BertForSequenceClassification.from_pretrained("bert-base-uncased", num_labels=2)

---

5️⃣ Evaluation Metrics

- Accuracy
- Precision
- Recall
- F1 Score
- Confusion Matrix

---

## 📊 Results

✅ Accuracy

~92% on test dataset

## 📉 Confusion Matrix Insights

- High True Positives & True Negatives
- Balanced performance across classes
- Low misclassification rate

---

## 🔥 Key Learnings

- Understanding transformer-based models
- Fine-tuning pre-trained models
- Handling large NLP datasets
- Evaluating classification models effectively

---

## 🚀 Future Improvements

- Hyperparameter tuning
- Using larger models (RoBERTa, DistilBERT)
- Deploying as a web app (Streamlit / Flask)

---

## 💡 How to Run

pip install transformers datasets torch scikit-learn matplotlib seaborn

Then open the notebook:

jupyter notebook bert-imdb-sentiment-analysis.ipynb

---
