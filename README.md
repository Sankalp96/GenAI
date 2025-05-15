# GenAI

# 🧠 MiniGPT: A Character-Level Transformer Language Model

This project is a minimalist implementation of a **character-level Transformer language model**, trained on Shakespeare’s works. Inspired by Andrej Karpathy’s `nanoGPT`, the model learns to generate text one character at a time.

---

## 📚 Overview

This model:
- Uses **Transformer blocks** with self-attention
- Learns from raw text using character-level tokenization
- Trains to predict the **next character**
- Can generate novel Shakespeare-like text after training

---

## 🏗️ Model Architecture

- **Token Embeddings**: Learns a vector for each character.
- **Positional Embeddings**: Encodes position of each character in a sequence.
- **Transformer Blocks**: Each block contains:
  - Multi-head self-attention (masked)
  - Feedforward layer
  - Layer normalization and residual connections
- **Output Layer**: Predicts the next character using a linear layer.

---

## ⚙️ Hyperparameters

```python
batch_size = 16
block_size = 32
n_embd = 64
n_head = 4
n_layer = 4
dropout = 0.0
learning_rate = 1e-3






