# 🧠 Sherlock Holmes Text Generation using LSTM (PyTorch)

## 📌 Project Overview

This project implements a word-level LSTM-based Language Model using PyTorch to generate text in the style of *Sherlock Holmes*.

The model is trained on:

📖 The Adventures of Sherlock Holmes by Arthur Conan Doyle  
(Source: Project Gutenberg)

The goal is to learn sequential word dependencies and perform next-word prediction, a foundational task in Natural Language Processing.

---

## 🎯 Objective

Given an input sequence:

"I was returning from"

The model predicts the most probable next word.

This is a Next-Word Prediction / Language Modeling task using LSTM (Long Short-Term Memory) networks.

---

## 🛠 Tech Stack

- Python
- PyTorch
- NLTK
- NumPy
- GPU support (if available)

---

## 📂 Dataset

- Full text corpus of The Adventures of Sherlock Holmes
- Preprocessing steps:
  - Lowercasing
  - Tokenization
  - Vocabulary creation
  - Handling unknown words (<unk>)
  - Sequence generation
  - Padding for batch processing

---

## 🧠 Model Architecture

Embedding Layer
      ↓
LSTM Layer
      ↓
Fully Connected Layer
      ↓
Softmax (via CrossEntropyLoss)

### Architecture Details

- Embedding Size: 100  
- Hidden Size: 150  
- LSTM Layers: 1  
- Loss Function: CrossEntropyLoss  
- Optimizer: Adam  

---

## 🔄 Training Process

1. Convert text into token sequences  
2. Create progressive n-gram sequences  
3. Pad sequences to uniform length  
4. Split into input and target  
5. Train LSTM to predict next word  
6. Generate text using greedy decoding  

---


## 🧪 Key Concepts Demonstrated

- Word Embeddings
- Recurrent Neural Networks (RNN)
- LSTM Architecture
- Custom PyTorch Dataset
- DataLoader usage
- Sequence Padding
- Text Generation
- Language Modeling fundamentals

---

## 🚀 Possible Improvements

- Add Train / Validation split
- Calculate Perplexity metric
- Implement Gradient Clipping
- Add Dropout for regularization
- Compare LSTM vs GRU
- Implement Temperature-based sampling
- Try Character-level modeling
- Add multi-layer LSTM

---

## 🎓 Learning Outcome

This project builds foundational understanding of:

- Sequential modeling
- Deep learning for NLP
- Next-token prediction
- Text generation systems

It serves as a stepping stone toward:
- GPT-style transformers
- Chatbots
- Machine Translation
- Autocomplete systems

---

## 👨‍💻 Author

Rick  
B.Tech CSE Student  
Aspiring Machine Learning Researcher
