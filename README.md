# 📜 Next Word Prediction using LSTM on Shakespeare's Hamlet

This project builds a next-word prediction model trained on Shakespeare’s *Hamlet* using an LSTM-based deep learning architecture. The model learns language structure and can generate the next word given an input phrase, offering a simple glimpse into the world of text generation and language modeling.

---

## 🔍 Objective

To develop a language model capable of understanding the context and predicting the **next word** in a sequence, based on the **Hamlet** corpus.

---

## 🛠️ Features

- Download and preprocess Shakespeare's *Hamlet* text using NLTK
- Tokenize and generate n-gram sequences
- Prepare input-output sequences for supervised training
- Train an LSTM-based text generation model
- Predict the next word given any valid input

---

## 📁 Project Structure

experiments.ipynb # Main notebook with code and training pipeline
hamlet.txt # Cleaned and preprocessed text of Hamlet
README.md # Project documentation



---

## 🧠 Model Architecture

- **Embedding Layer** – Converts tokens to dense vectors
- **LSTM Layers** – Captures temporal dependencies in text
- **Dropout Layer** – Regularizes the model
- **Dense Output Layer** – Predicts next word (softmax across vocabulary)

---

## 📊 Results

| Metric            | Value (Sample) |
|-------------------|----------------|
| Training Accuracy | ~90%           |
| Validation Loss   | Low            |

> _Note: Actual results may vary depending on training time and system configuration._

---

## 🧪 Sample Usage

```python
input_text = "To be or"
next_word = predict_next_word(model, tokenizer, input_text, max_sequence_len)
print(f"Next word prediction: {next_word}")
