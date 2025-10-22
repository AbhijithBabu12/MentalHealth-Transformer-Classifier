# 🧠 Mental Health Text Classification using Mini Transformer

This project implements a **custom Transformer-based NLP model** to classify mental health–related text statements into multiple categories such as anxiety, depression, neutral, and more.  
Built entirely from scratch in **PyTorch**, the model leverages **multi-head self-attention**, **positional encoding**, and **feed-forward layers** to learn contextual emotional patterns in text data.

---

## 🚀 Project Overview

| Feature | Description |
|----------|-------------|
| **Model Type** | Custom Transformer Encoder |
| **Dataset** | Mental health text dataset (`mental.csv`) |
| **Task** | Multi-class Text Classification |
| **Framework** | PyTorch |
| **Accuracy** | ~71% on Test Set |
| **Classes** | 7 mental health categories |

---

## 🧩 Model Architecture

The model consists of:
- **Embedding Layer** — Converts tokens into dense vectors.  
- **Positional Encoding** — Adds sequence order information to embeddings.  
- **Transformer Encoder Layers** — Utilize *multi-head self-attention* and *layer normalization* to capture global dependencies.  
- **Feed-Forward Network** — Expands and projects features.  
- **Mean Pooling + Linear Layer** — Aggregates sequence info for final classification.

---

## 📊 Results

| Metric | Value |
|:-------|:------:|
| **Test Accuracy** | **0.71** |
| **Macro F1-score** | **0.69** |
| **Weighted F1-score** | **0.73** |

> Achieved consistent performance across 7 classes, with the Transformer outperforming traditional RNN-based baselines on contextual statements.

---

## ⚙️ Training Configuration

| Parameter | Value |
|------------|-------|
| Embedding Dim | 128 |
| Heads | 8 |
| FF Hidden Dim | 256 |
| Layers | 3 |
| Learning Rate | 1e-3 |
| Epochs | 10 |
| Batch Size | 32 |

---

## 🧠 Sample Predictions

```text
"I feel great and happy today!" → positive / healthy  
"This is so frustrating and bad" → negative / stress  
"Feeling excited to see friends" → cheerful / active  
```
---

## 👨‍💻 Author

Abhijith Babu
Passionate about ML & AI 🚀

📌 GitHub: [https://github.com/AbhijithBabu12]

📌 LinkedIn: [https://www.linkedin.com/in/abhijith-babu-856170201/]
