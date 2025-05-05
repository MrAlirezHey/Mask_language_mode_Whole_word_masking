# Mask_language_mode_Whole_word_masking
Masked Language Modeling with DistilBERT on IMDB Dataset using Whole Word Masking

This project fine-tunes a lightweight BERT variant, DistilBERT, on the IMDB movie review dataset using the Masked Language Modeling (MLM) objective. To enhance the linguistic consistency of masked tokens, we applied Whole Word Masking (WWM) instead of standard token-level masking.

🔧 Key Features:

Dataset: IMDB (repurposed for unsupervised pretraining)

Model: DistilBERT (distilbert-base-uncased)

Objective: Masked Language Modeling (MLM)

Masking Strategy: Whole Word Masking with 20% probability

Custom data collator with WWM logic

Evaluation metrics: Loss and Perplexity

Trainer API used with optional FP16 mixed-precision training

⚠️ Note:
While IMDB is not a typical pretraining dataset (like Wikipedia), it still allows the model to learn domain-specific patterns of natural language in movie reviews.

# 🧠 Masked Language Modeling with DistilBERT on IMDB (Whole Word Masking)

This project fine-tunes [DistilBERT](https://huggingface.co/distilbert-base-uncased) on the IMDB movie reviews dataset using the **Masked Language Modeling (MLM)** objective. It uses **Whole Word Masking (WWM)** instead of standard token-level masking to enhance contextual consistency during training.

---

## 📚 Overview

- **Model:** `distilbert-base-uncased`
- **Dataset:** IMDB (adapted for unsupervised MLM)
- **Task:** Masked Language Modeling (MLM)
- **Masking:** Whole Word Masking (WWM) with 20% probability
- **Training API:** 🤗 HuggingFace `Trainer`
- **Evaluation Metrics:** Loss, Perplexity

---

## 🛠️ Installation

Make sure you have Python 3.7+ and install the required libraries:

```bash
pip install transformers datasets numpy
