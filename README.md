# Twitter Tweets Sentiment Analysis

A machine learning-based sentiment classification project that uses **TF-IDF feature extraction and Logistic Regression** to classify Twitter tweets into positive and negative sentiment classes.

## Overview

This project analyzes Twitter data and applies text preprocessing and machine learning techniques to classify tweets based on their sentiment.

The text is cleaned using tokenization, stopword removal, and lemmatization before being converted into numerical features using TF-IDF. A Logistic Regression classifier is then trained to predict the sentiment of unseen tweets.

## Approach

* Loaded and explored the Twitter dataset.
* Removed URLs, mentions, hashtags, and punctuation from tweets.
* Tokenized the text using NLTK.
* Removed English stopwords.
* Applied WordNet lemmatization.
* Converted cleaned tweets into TF-IDF feature vectors.
* Limited the feature representation to the top 5,000 features.
* Split the dataset into training and testing sets using an 80:20 split.
* Trained a Logistic Regression classifier.
* Evaluated the model using accuracy, precision, recall, F1-score, and a confusion matrix.

## Model

**Feature Extraction:** TF-IDF Vectorization
**Classifier:** Logistic Regression

The Logistic Regression model achieved an overall **accuracy of 95%** on the test set.

### Classification Results

| Class                | Precision | Recall | F1-Score |
| -------------------- | --------: | -----: | -------: |
| 0                    |      0.95 |   1.00 |     0.97 |
| 1                    |      0.91 |   0.35 |     0.50 |
| **Overall Accuracy** |           |        | **0.95** |

The results show strong overall accuracy, while the lower recall for class 1 indicates that the model has difficulty identifying some instances of the positive class.

## Data Visualization

The project includes:

* **Confusion Matrix** to visualize predicted versus true sentiment labels.
* **Classification Report Heatmap** to visualize precision, recall, and F1-score for each class.

## Tech Stack

**Language:** Python

**Libraries:** Pandas, NLTK, Scikit-learn, Matplotlib, Seaborn

**Techniques:** Text Preprocessing, Tokenization, Stopword Removal, Lemmatization, TF-IDF, Logistic Regression

## Dataset

The project uses a Twitter dataset containing:

* `id` — Tweet identifier
* `label` — Sentiment label
* `tweet` — Tweet text

# Results:
![Confusion Matrix](https://github.com/ruchira30/Twitter-Tweets-Sentiment-Analysis/blob/main/confusion_matrix.png)
![Classification Report](https://github.com/ruchira30/Twitter-Tweets-Sentiment-Analysis/blob/main/classification_report.png)

## Author

**Ruchira Purohit**

