# 🎬 Movie Review Sentiment Classifier (AWD-LSTM)

A high-performance sentiment analysis model built using **Fastai** and **PyTorch**. This project implements the **ULMFiT** (Universal Language Model Fine-tuning) approach to achieve state-of-the-art results on the IMDB Movie Reviews dataset.

[![Fastai](https://img.shields.io/badge/Library-Fastai-blue)](https://docs.fast.ai/)
[![PyTorch](https://img.shields.io/badge/Framework-PyTorch-red)](https://pytorch.org/)
[![Accuracy](https://img.shields.io/badge/Accuracy-93%25-brightgreen)](#)

## 📌 Project Overview
This project goes beyond traditional machine learning by utilizing a Deep Learning architecture known as **AWD-LSTM** (Asynchronous Weight-dropped LSTM). By leveraging Transfer Learning, the model understands linguistic context and nuances, reaching an accuracy of **93%**.

### **Key Highlights:**
* **Dataset:** IMDB (Large Movie Review Dataset)
* **Architecture:** AWD-LSTM 
* **Methodology:** ULMFiT (3-stage Fine-tuning)
* **Performance:** 93% Validation Accuracy

---

## 🧠 Technical Deep Dive: The ULMFiT Strategy

Instead of training a model from scratch, I followed the **ULMFiT** pipeline:

1. **General Language Model Pre-training:** Utilized a model pre-trained on the Wikipedia (Wikitext-103) dataset to understand English grammar.
2. **Target Task LM Fine-tuning:** Fine-tuned the Language Model specifically on the IMDB dataset. This allows the model to learn the specific "slang" and vocabulary used by movie critics.
3. **Sentiment Classifier:** The final stage where the encoder is attached to a classifier head to predict **Positive** or **Negative** labels.

### **Why AWD-LSTM?**
AWD-LSTM is specifically designed to handle the vanishing gradient problem in long sequences (like movie reviews) while using various dropout techniques (Weight Dropout, Embedding Dropout) to ensure the model doesn't overfit.

---

## 🛠️ Tech Stack
* **Language:** Python
* **Libraries:** Fastai v2, PyTorch, Pandas, NumPy
* **Training Environment:** [Insert: e.g., Google Colab / Kaggle]

---

## 📂 Project Structure
```text
├── Movie_Sentiment_AWD_LSTM.ipynb  # Main Jupyter Notebook
├── export.pkl                      # Exported Model weights (Learner object)
├── data/                           # (Optional) IMDB dataset folder
└── README.md                       # Project Documentation
