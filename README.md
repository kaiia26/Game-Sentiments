# Steam Reviews Sentiment Analysis Pipeline

This project implements a scalable NLP preprocessing pipeline for **17,000+ Steam reviews**, designed to clean and transform textual and numeric data into a format suitable for **sentiment analysis**, classifying reviews as positive or negative based on their wording.

---

## Features

- **Text Cleaning & Normalization**
  - Regex-based cleaning (`re`) to remove punctuation, special characters, and unwanted text patterns.
  - Stopword removal using NLTK.
  - Lemmatization with NLTK's `WordNetLemmatizer` to standardize word forms.
  - Numeric and date conversion to words using `num2words` and `inflect` for consistency.
  
- **Batch Processing for Efficiency**
  - Handles large datasets in batches depending on the number of cpu cores, efficiently converting numeric and date fields into textual format.
  - Significantly reduces preprocessing time from ~10 minutes to under 2 minutes per batch.
 
- **Data Handling & Analysis**
  - `pandas` for structured data handling, cleaning, and transformation.
  - `numpy` for efficient numerical operations and array manipulation.
  - `matplotlib` for visualizing distributions, review lengths, and sentiment patterns during exploratory data analysis.

- **Feature Extraction & ML-Ready Output**
  - TF-IDF vectorization using `scikit-learn` for textual features.
  - Label encoding for categorical data.
  - Outputs cleaned, preprocessed text suitable for classification or other NLP tasks.

---

## Tech Stack

- **Language:** Python  
- **Libraries:**  
  - `pandas`, `numpy` – Data manipulation  
  - `scikit-learn` – Preprocessing, vectorization, modeling  
  - `nltk` – Tokenization, stopword removal, lemmatization  
  - `num2words`, `inflect` – Numeric to text conversion  
  - `kaggle`, `kagglehub` – Data acquisition and management  
