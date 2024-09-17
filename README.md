Fake News Detection with PassiveAggressiveClassifier
This project implements a machine learning model to detect fake news using the PassiveAggressiveClassifier algorithm. The model is trained and tested on a news dataset, with the text features vectorized using TfidfVectorizer. The aim is to classify news articles as either REAL or FAKE.

Table of Contents:
  - Introduction
  - Dataset
  - Project Workflow
  - Modeling
  - Results

Introduction

Fake news is a growing concern in today’s digital age, where misleading information can spread rapidly. This project builds a simple but effective machine learning pipeline to classify news articles as REAL or FAKE. The model leverages the TfidfVectorizer to transform the news text into feature vectors, and uses PassiveAggressiveClassifier to train a binary classifier that can differentiate between fake and real news.
The model achieves an accuracy of 92.9% and has been evaluated using a confusion matrix.

Dataset
The dataset used in this project is a CSV file (news.csv) that contains the following columns:
  - title: The title of the news article.
  - text: The body content of the news article.
  - label: The label indicating whether the news article is REAL or FAKE.
  - The dataset contains 6335 rows and 4 columns.


Project Workflow

1. Data Preprocessing:
   Load the dataset using pandas.
   Split the data into training and testing sets.

2. Text Vectorization:
   Use TfidfVectorizer to convert the text data into numerical feature vectors.

3. Modeling:
   Train a PassiveAggressiveClassifier on the vectorized training data.
   Evaluate the model on the test data to calculate accuracy and create a confusion matrix.

4. Performance Evaluation:
   Calculate the model’s accuracy.
   Generate and visualize the confusion matrix.

Results

Accuracy: The model achieved an accuracy of 92.9% on the test set.

Confusion Matrix:
[[591,  47],
 [ 43, 586]]

This shows that out of 1267 news articles in the test set:
  - 591 were correctly classified as FAKE.
  - 586 were correctly classified as REAL.
  - 47 FAKE news articles were misclassified as REAL.
  - 43 REAL news articles were misclassified as FAKE.


