# 🎬 IMDB Movie Reviews Sentiment Analysis (NLP & Deep Learning)

![Python](https://img.shields.io/badge/Python-3.8%2B-blue.svg)
![Framework](https://img.shields.io/badge/PyTorch-HuggingFace-orange.svg)
![TensorFlow](https://img.shields.io/badge/TensorFlow-Keras-red.svg)
![Accuracy](https://img.shields.io/badge/BERT%20Accuracy-91.37%25-brightgreen.svg)
![License](https://img.shields.io/badge/License-MIT-green.svg)

An end-to-end Natural Language Processing (NLP) project that evaluates and classifies IMDB movie reviews as either **Positive** or **Negative**. This project benchmarks classical Machine Learning algorithms, Deep Learning architectures (LSTM), and state-of-the-art Transformer models (**BERT**).

---

## 📌 Table of Contents
- [Project Overview](#-project-overview)
- [Dataset Information](#-dataset-information)
- [Project Architecture & Workflow](#-project-architecture--workflow)
- [Models & Performance Benchmark](#-models--performance-benchmark)
- [Tech Stack](#-tech-stack)
- [Installation & Local Setup](#-installation--local-setup)
- [Project Structure](#-project-structure)
- [Future Roadmap](#-future-roadmap)
- [Author](#-author)

---

## 📌 Project Overview

Understanding sentiment from user reviews provides business intelligence for streaming platforms, e-commerce applications, and entertainment analytics. This project explores the **IMDB 50k Dataset** to build and compare three distinct NLP pipelines:

1. **TF-IDF + Logistic Regression**: A fast, interpretable classical Machine Learning baseline.
2. **LSTM (Long Short-Term Memory)**: A recurrent neural network designed to capture sequential word dependencies.
3. **Fine-Tuned BERT (`bert-base-uncased`)**: A bi-directional transformer model leveraging transfer learning for high accuracy.

---

## 📊 Dataset Information

- **Name**: IMDB Dataset of 50K Movie Reviews
- **Total Samples**: 50,000 reviews
- **Distribution**: 25,000 Positive / 25,000 Negative (100% Balanced)
- **Task**: Binary Text Classification (`1` = Positive, `0` = Negative)

---

## ⚙️ Project Architecture & Workflow

```text
[ Raw Text Data ] ➡️ [ Regex Cleaning & Preprocessing ] ➡️ [ Tokenization & Encoding ]
                                                                     │
        ┌──────────────────────────────┬─────────────────────────────┴─────────────────────────────┐
        ▼                              ▼                                                           ▼
[ Classical Pipeline ]        [ Deep Learning Pipeline ]                                  [ Transformer Pipeline ]
  • TF-IDF Vectorizer           • Keras Tokenizer                                           • BERT Tokenizer
  • Logistic Regression         • Sequence Padding                                          • Fine-Tuned PyTorch Model
        │                              │                                                           │
        ▼                              ▼                                                           ▼
  Accuracy: 89.76%              Sequential LSTM                                             Accuracy: 91.37%

👤 Author
Md Nahidul Islam
Graduate Student, Department of Computer Science & Engineering
Green University of Bangladesh

If you find this repository useful, feel free to give it a ⭐!
