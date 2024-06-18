# Amazon-Reviews-using-Sentiment-Analysis

## Business Problem

1. **Identify Product Categories with Lower Reviews**: Determine which product categories (e.g., electronics, iPads) have lower reviews, indicating potentially inferior products.
2. **Identify Product Categories with Higher Reviews**: Determine which products have higher reviews, indicating potentially superior products.

### Business Solutions

1. **Product Roster Management**: Identify which products should be kept or dropped from Amazon's product roster based on review sentiment.
2. **Sentiment Association**: Associate positive and negative words/sentiments with each product in Amazon's catalog.
3. **Predictive Sentiment Analysis**: Predict review scores based on specific words using sentiment analysis.

### Dataset Focus

This dataset is based on Amazon-branded/Amazon-manufactured products. The primary focus is on customer satisfaction with Amazon products.

### Potential Product Review Suggestions

Example: 
- *Product X is highly rated on the market, with most people appreciating its lightweight, sleek design, and fast speeds. Negative reviews often mention it being too heavy and difficult to fit in bags. We suggest that next-gen models for e-readers should be lightweight and portable, based on this data.*

### Assumptions

1. **Sample Size**: A sample size of 30K examples is assumed to be sufficient to represent the entire population of sales/reviews.
2. **Richness of Information**: The text reviews of each product are assumed to be rich enough to train a sentiment analysis classifier with an accuracy of hopefully >70%.

## Table of Contents

1. [Introduction](#introduction)
2. [Setup](#setup)
3. [Data Preparation](#data-preparation)
4. [Feature Extraction](#feature-extraction)
5. [Model Training](#model-training)
6. [Model Evaluation](#model-evaluation)
7. [Fine-tuning](#fine-tuning)
8. [Detailed Performance Analysis](#detailed-performance-analysis)
9. [Conclusion](#conclusion)

## Introduction

This project aims to build a robust sentiment analysis system to classify product reviews into positive, neutral, and negative sentiments using various machine learning models.

## Setup

To set up the environment, follow these steps:

1. Clone the repository:
    ```bash
    git clone https://github.com/yourusername/sentiment-analysis.git
    cd sentiment-analysis
    ```

2. Create a virtual environment and activate it:
    ```bash
    python -m venv venv
    source venv/bin/activate  # On Windows, use `venv\Scripts\activate`
    ```

3. Install the required packages:
    ```bash
    pip install -r requirements.txt
    ```

## Data Preparation

1. **Load the dataset**: Import the dataset containing product reviews and ratings.

2. **Categorize ratings into sentiments**: Convert numerical ratings into categorical sentiments (positive, neutral, negative).

3. **Prepare the data**: Separate the review texts and their corresponding sentiments for training and testing.

## Feature Extraction

1. **Convert text data into numerical feature vectors**: Use techniques such as Count Vectorizer and TF-IDF to transform text data into numerical representations that machine learning models can process.

## Model Training

1. **Train various classifiers**: Implement and train different machine learning models (e.g., Multinomial Naive Bayes, Logistic Regression, Support Vector Machines, Decision Trees, Random Forests) using the extracted features.

## Model Evaluation

1. **Evaluate the models**: Test the trained models on the test dataset and compare their performance using metrics like accuracy.

2. **Choose the best performing model**: Identify the model with the highest accuracy or other relevant performance metrics.

## Fine-tuning

1. **Fine-tune the best performing model**: Use techniques such as Grid Search to optimize the hyperparameters of the best performing model to avoid overfitting and improve performance.

## Detailed Performance Analysis

1. **Analyze performance metrics**: Generate detailed classification reports and confusion matrices to evaluate precision, recall, F1-score, and support for each class.

2. **Interpret results**: Understand the strengths and weaknesses of the model, especially in handling skewed data distributions.

## Conclusion

The sentiment analysis system developed in this project successfully classifies product reviews with high accuracy. Despite the dataset being skewed towards positive reviews, the machine learning models perform well in predicting sentiments. The model's performance can further improve with more balanced data. This project demonstrates the potential of using machine learning for sentiment analysis in real-world applications.

