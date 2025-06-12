# Development of an Automatic Sentiment Analysis Tool for Urdu Text

**A complete NLP pipeline for Urdu social media text—preprocessing, feature extraction, and sentiment classification.**

---

## 🔍 Table of Contents

- [Overview](#overview)  
- [Features](#features)  
- [Dataset](#dataset)  
- [Installation](#installation)  
- [Usage](#usage)  
- [Pipeline Details](#pipeline-details)  
- [Evaluation](#evaluation)  
- [Challenges](#challenges)  
- [Future Work](#future-work)  
- [Contributing](#contributing)  
- [License](#license)

---

## Overview

This project builds an end-to-end sentiment analysis pipeline for Urdu social media texts, targeting platforms like Twitter and YouTube. It classifies text into **positive**, **negative**, or **neutral** sentiments, helping brands and businesses interpret feedback in Urdu.

---

## Features

1. **Text Preprocessing**
   - Custom stopword removal with sentiment retention  
   - Text cleaning (punctuation, URLs, emojis, hashtags)  
   - Emoji-to-sentiment mapping  
   - Filtering posts shorter than three words  

2. **Morphological Processing**
   - Urdu stemming  
   - Urdu lemmatization  

3. **Feature Extraction**
   - Tokenization for Urdu text  
   - TF–IDF vectorization with top-term extraction  
   - Word2Vec embedding model with similarity queries  

4. **N‑Gram Analysis**
   - Extraction of unigrams, bigrams, and trigrams  
   - Frequency-based ranking of top 10 for bigrams/trigrams  

5. **Sentiment Classification**
   - Multinomial Naive Bayes using TF–IDF features  
   - Evaluation metrics: accuracy, precision, recall, F1-score  

---

## Dataset

Uses a publicly available Urdu social media dataset (e.g., Kaggle’s Urdu Twitter Sentiment Dataset).  
Ensure the dataset CSV includes:
- `urdu_text`: raw Urdu post
- `is_sarcastic`: sentiment label (`0`, `1`, etc.)  
*(Adapt columns if using another dataset.)*

---

## Installation

```bash
git clone https://github.com/<your-username>/urdu-sentiment-analysis.git
cd urdu-sentiment-analysis
pip install -r requirements.txt
