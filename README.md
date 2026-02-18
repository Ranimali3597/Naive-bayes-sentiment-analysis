# Naive-bayes-sentiment-analysis
This project implements a complete Sentiment Analysis Classifier using the Naive Bayes algorithm, built entirely from scratch without using machine-learning libraries such as scikit-learn. The goal of the project is to classify tweets as positive or negative, based on their textual content. 
By manually computing probabilities and applying NLP techniques, this project provides a deep understanding of how Naive Bayes works behind the scenes.

The dataset used in this project contains approximately 500 tweets, each labeled as either positive (1) or negative (0). The main focus of the project is to process this raw text data, extract meaningful patterns, and build a working classification model step by step.

The workflow begins with data preprocessing, where tweets are cleaned by converting text to lowercase, removing punctuation, filtering stopwords, and tokenizing the words. After preprocessing, the model creates a frequency dictionary that stores how often each word appears in positive and negative tweets. This dictionary becomes the core of the Naive Bayes probability calculations.

Next, the model computes two major components:

Log Prior – the log ratio of positive to negative tweets in the dataset

Log Likelihood – the log ratio of how likely each word is to appear in positive versus negative tweets

These values are then used to train the Naive Bayes classifier. For prediction, the model evaluates new tweets by summing the log likelihoods of each word along with the log prior. If the final score is greater than zero, the tweet is classified as positive; otherwise, negative.

The project also includes model testing, accuracy evaluation, and error analysis to understand which tweets are misclassified and why. Additionally, it allows users to input their own tweets and see the sentiment prediction in real time.

This project is ideal for anyone who wants to understand the mathematical foundation of Naive Bayes, learn text preprocessing in NLP, and build a sentiment classifier without relying on pre-built ML libraries. Future enhancements may include Streamlit deployment, dataset expansion, and comparison with other algorithms.
Project Features

Preprocess tweets (lowercasing, cleaning, removing punctuation & stopwords)

Build word-frequency dictionary

Compute:

Log Prior

Log Likelihood

Train a Naive Bayes classifier for sentiment prediction

Test model accuracy

Error analysis

Predict on your own text input
