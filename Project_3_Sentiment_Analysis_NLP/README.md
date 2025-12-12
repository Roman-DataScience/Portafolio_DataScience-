# 💬 Project 3: Sentiment Analysis (NLP)

## Executive Summary
This project demonstrates the fundamental pipeline for Natural Language Processing (NLP) by classifying customer reviews as Positive (1) or Negative (0). It showcases essential text preprocessing and machine learning techniques for text classification.

## 🎯 Objective
To build a classification model to determine the sentiment (positive or negative) of a movie review using the Multinomial Naive Bayes algorithm.

## ⚙️ Methodology & Techniques
* **Text Preprocessing (Cleaning):** Implemented a robust function to clean text, including: **Tokenization**, conversion to **lowercase**, removal of **stop words**, removal of **punctuation and numbers**, and filtering words by **length**.
* **Feature Extraction:** Used **TF-IDF (Term Frequency-Inverse Document Frequency)** to vectorize the clean text, transforming words into numerical features weighted by their importance across the dataset.
* **Model Training:** Trained a **Multinomial Naive Bayes** model, which is highly effective for text classification tasks based on word counts/frequencies.
* **Model Interpretation:** Calculated the **Log-Ratio** of feature probabilities to identify the top 10 most **positive** and top 10 most **negative** predictive words in the vocabulary.

## 📊 Key Findings
* **Model Performance (Accuracy):** The model achieved a prediction accuracy of **0.7634** on the test set.
* **Top Predictive Words:** The analysis successfully isolated highly influential words, such as 'great', 'love', and 'excellent' for positive sentiment, and 'worst', 'bad', and 'waste' for negative sentiment.

---
**[View Notebook: Analisis_Sentimiento_NB.ipynb](Analisis_Sentimiento_NB.ipynb)**
