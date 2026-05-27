# Steam Reviews Aspect-Based Sentiment Analysis Pipeline

This project implements a natural language processing pipeline for **17,000+ Steam game reviews**, focused on cleaning noisy user-generated text and preparing it for **Aspect-Based Sentiment Analysis (ABSA)**.

Unlike traditional sentiment analysis, which predicts a single overall sentiment, this project aims to identify sentiment toward specific gameplay-related aspects such as graphics, gameplay, monetization, performance, controls, and multiplayer experience.

---

## Features

### **Text Cleaning & Normalization**

* Regex-based preprocessing using Python’s `re` library to normalize noisy gaming-related review text.
* URL removal, punctuation cleanup, and whitespace normalization.
* Cleaning of corrupted alphanumeric tokens and embedded digit patterns commonly found in Steam reviews.
* Numeric-to-text conversion using `num2words`.
* Tokenization using NLTK for downstream NLP processing.

---

### **Gaming Slang & Abbreviation Handling**

* Custom preprocessing rules for gaming-specific abbreviations and slang:

  * `p2w → pay to win`
  * `fps → first person shooter`
  * `f2p → free to play`
  * `tf2 → team fortress two`
* Handling of punctuation-heavy and shorthand user-generated text commonly found in online gaming communities.

---

### **Exploratory Data Analysis**

* Used `pandas` and `numpy` for structured preprocessing and data transformation.
* Used `matplotlib` to analyze review distributions, review lengths, and token patterns.
* Built regex-based inspection utilities to identify malformed tokens, URLs, special characters, and uncommon vocabulary.

---

### **Aspect-Based Sentiment Analysis (ABSA)**

* Preparing tokenized Steam reviews for aspect-level sentiment classification.
* Identifying review sentiment associated with gameplay-related aspects such as:

  * gameplay
  * graphics
  * monetization
  * controls
  * multiplayer experience
  * performance
* Building an NLP workflow for fine-grained sentiment analysis on gaming review data.

---

## Tech Stack

* **Language:** Python

* **Libraries:**

  * `pandas`, `numpy` — data manipulation and preprocessing
  * `scikit-learn` — machine learning utilities and evaluation
  * `nltk` — tokenization and NLP preprocessing
  * `matplotlib` — exploratory data visualization
  * `num2words` — numeric-to-text conversion
  * `kaggle`, `kagglehub` — dataset acquisition and management

