# Sentiment Analysis on Amazon Product Reviews

## Overview
This project performs sentiment analysis on Amazon product reviews to predict whether a review is positive (1) or negative (0) based on the review text.

## Dataset
- Source: Amazon product reviews dataset
- Features: Review text
- Target: Sentiment (Positive=1, Negative=0)
- No missing values

## Models Used
- Random Forest
- Support Vector Machine (SVM)
- Naive Bayes
- LSTM (Deep Learning)

## Text Preprocessing
- Lowercase conversion
- Remove punctuation and special characters
- Tokenization
- Stop words removal
- Lemmatization
- TF-IDF vectorization
- Word2Vec embeddings

## Results

| Model | Accuracy | Precision | Recall | F1 Score |
|-------|----------|-----------|--------|----------|
| Random Forest | 0.867 | 0.870 | 0.970 | 0.917 |
| **SVM** | **0.889** | 0.897 | 0.965 | **0.930** |
| Naive Bayes | 0.799 | 0.792 | **0.997** | 0.883 |
| LSTM | 0.867 | **0.907** | 0.920 | 0.913 |

## Key Findings
- **Best Overall**: SVM with highest F1 score (0.930)
- **Best Precision**: LSTM (0.907) - fewest false positives
- **Best Recall**: Naive Bayes (0.997) - rarely misses positive reviews
- **Best Interpretability**: Random Forest with feature importance

## Requirements
- Python 3.x
- pandas, numpy, matplotlib, seaborn
- nltk, gensim
- scikit-learn
- tensorflow, keras, keras-tuner
