# Sentiment Analysis of IMDB Movie Reviews

This project performs sentiment analysis on IMDB movie reviews using **Word2Vec** and a **Random Forest Classifier**. The goal is to predict whether a review is **positive** or **negative** based on the text of the review.

## Project Overview

In this project, we use Natural Language Processing (NLP) techniques to preprocess the IMDB movie dataset and train a machine learning model to classify movie reviews as positive or negative. The project includes the following steps:

1. **Data Preprocessing**: Cleaning and preparing the data for analysis.
2. **Word2Vec**: Converting text into word embeddings to capture semantic meaning.
3. **Model Training**: Training a **Random Forest Classifier** to classify the reviews.
4. **Evaluation**: Evaluating the model's performance using accuracy and classification metrics.

## Dataset

The dataset used for this project is the **IMDB Movie Reviews** dataset. The dataset contains 50,000 reviews, with labels indicating whether the review is **positive** or **negative**.

You can download the dataset from [Kaggle - IMDB Dataset](https://www.kaggle.com/datasets/lakshmi25npathi/imdb-dataset-of-50k-movie-reviews).

### Dataset Format

- `review`: The text of the movie review.
- `sentiment`: The sentiment label (positive or negative).

## Steps

### 1. Data Preprocessing
The data preprocessing steps include:

- Removing **HTML tags** from the reviews.
- Converting all text to **lowercase**.
- Removing **stopwords** to eliminate common words that don’t contribute to sentiment.

### 2. Tokenization
We tokenize the reviews using the **nltk.word_tokenize** function. Tokenization splits the text into individual words.

### 3. Word2Vec Embeddings
We use the **Word2Vec** model from the **Gensim** library to convert the reviews into **word embeddings**. These embeddings represent the semantic meaning of the words in the reviews.

### 4. Training the Model
We use a **Random Forest Classifier** to train the model. The model is trained on the vectorized reviews and their corresponding sentiment labels.

### 5. Model Evaluation
The model is evaluated using **accuracy**, **precision**, **recall**, and **F1-score** metrics. 

