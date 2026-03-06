# Sarcasm-Aware Sentiment Analysis: A Hybrid Symbolic–Neural Pipeline 

## The Problem
Standard Transformer-based models often suffer from a **"Sarcasm Blind-spot."** Traditional models tend to latch onto keywords and fail to understand the context of the entire statement. 

> **Example:** *"Battery lasted 10 minutes. Absolute genius engineering!"*

While a human easily recognizes the sarcasm, a standard model will zero in on the phrase *"genius engineering"* and incorrectly predict a positive sentiment, completely ignoring the preceding factual complaint.

---

## The Solution
This project moves beyond end-to-end black-box modeling by implementing a **Hybrid Pipeline** that bridges deep learning with linguistic logic. By successfully isolating factual complaints from sarcastic sentiment, the system achieves a **95% Negative Recall** on sarcastic datasets.

---

## Key Technical Features

* **Discourse-Based Logical Slicing:** Uses advanced text segmentation to decouple factual premises from sentiment-heavy conclusions.
* **Incongruity Detection:** A Zero-Shot NLI (Natural Language Inference) layer that flags logical contradictions between different segments of a text.
* **Incongruity Rule Engine:** Automatically inverts sentiment scores if a negative fact is paired with positive praise without standard transition markers (e.g., "but", "however").
* **Weighted Verdict Optimization:** Implements a Grid Search-optimized weighting system (1.75x) for the decisive verdict segments to ensure accurate final classification.
* **Brand Intelligence Dashboard:** Features a **"Sarcasm Index"** tracker to filter out noise, helping businesses identify genuine brand loyalty versus sarcastic criticism.

---

## Tech Stack

* `Python`
* `HuggingFace Transformers`
* `Spacy`
* `NLTK`
* `Scikit-Learn`
* `Zero-Shot Classification`

---
## Infographic
<img width="1024" height="559" alt="image" src="https://github.com/user-attachments/assets/8db063bc-76bf-4ae8-99ce-933d703902ff" />

