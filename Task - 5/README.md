# 🧠 POS Tagging & Chunking using BERT (Token Classification)

## 📌 Project Overview

This project focuses on building a token classification system using Transformer models to perform:

- ✅ Part-of-Speech (POS) Tagging
- ✅ Chunking (Phrase Detection)

Using DistilBERT, the model is fine-tuned to understand the structure of language at both word-level and phrase-level.

---

## 🎯 Objective

The goal of this project is to:

- Understand token classification using Transformers
- Perform sequence labeling tasks like POS tagging and chunking
- Handle challenges such as subword tokenization and label alignment
- Evaluate model performance using sequence-based metrics

---

## 🛠️ Tech Stack

- Python
- Hugging Face Transformers
- PyTorch
- NLTK (for dataset)
- SeqEval (for evaluation)
- Google Colab

---

## 📂 Dataset

- CoNLL-2000 Dataset (via NLTK)
- Contains:
  - Words
  - POS Tags
  - Chunk Tags

Example:

Confidence   NN   B-NP  
in           IN   B-PP  
the          DT   B-NP  

---

## ⚙️ Project Pipeline

Raw Data → Tokenization → Label Alignment → Model Training → Evaluation → Inference → Comparison

---

## 🔍 Data Preprocessing

- Tokenization using BERT tokenizer
- Alignment of labels with tokens
- Handling:
  - Subwords using "-100"
  - Special tokens
  - Padding & truncation

---

## 🤖 Model

- Model Used: "distilbert-base-uncased"
- Task: Token Classification
- Library: "AutoModelForTokenClassification"

---

## 🚀 Training Details

- Epochs: 3
- Batch Size: 16
- Learning Rate: 2e-5
- Optimizer: AdamW (default Hugging Face)

---

## 📊 Evaluation Results

POS Tagging Performance:

- Precision: 0.9650
- Recall: 0.9670
- F1 Score: 0.9660
- Accuracy: 0.9754

✔️ Achieved strong performance using Transformer-based approach.

---

## 🧪 Inference Example

Input:

John works at Google in California

Output:

John        → NNP  
works       → VBZ  
Google      → NNP  
California  → NNP  

---

## 🔄 POS Tagging vs Chunking

Aspect| POS Tagging| Chunking
Level| Word-level| Phrase-level
Complexity| Easier| Moderate
Output| Grammar tags| Phrase groups

---

## ⚠️ Challenges Faced

- Handling subword tokenization
- Aligning labels correctly with tokens
- Managing padding and sequence length
- Understanding sequence-based evaluation

---

## 📌 Observations

- Transformer models perform exceptionally well for NLP tasks
- Context-aware embeddings improve accuracy
- POS tagging is simpler compared to chunking
- Proper preprocessing is crucial for performance


---

## 📈 Future Improvements

- Use larger models like BERT-base
- Train for more epochs
- Deploy as an API
- Add visualization for predictions

---
