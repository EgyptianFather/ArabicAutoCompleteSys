# 🔮 Arabic Word-Level Autocomplete

This project is an **Arabic word-level autocomplete** system built using a trained neural network model and deployed with **Gradio**. It suggests the **most likely next word** after a user types and presses the spacebar.

---

## 📌 Features

- ✅ **Arabic word suggestions** after each word
- ✅ **Handles Arabic text preprocessing**
- ✅ **Skips unknown (`<UNK>`) tokens when predicting**
- ✅ **Gradio live interface**
- ✅ **Clean and minimal design**

---

## 🧠 Model Overview

- **Type**: Sequence model (e.g., LSTM or Transformer)
- **Input**: Sequence of words (as integer tokens)
- **Output**: Probability distribution over vocabulary for the next word

---

## 🧼 Preprocessing

We clean the Arabic text by:

- Removing **diacritics** (التشكيل)
- Removing **punctuation, digits, and Latin characters**
- Keeping Arabic letters **unchanged** (e.g., we do *not* normalize 'ؤ', 'ى', etc.)
