#Sentiment Analysis of IMDB Movie Reviews
This project performs sentiment analysis on IMDB movie reviews using Word2Vec and a Random Forest Classifier. The goal is to predict whether a review is positive or negative based on the text of the review.

Project Overview
In this project, we use Natural Language Processing (NLP) techniques to preprocess the IMDB movie dataset and train a machine learning model to classify movie reviews as positive or negative. The project includes the following steps:

Data Preprocessing: Cleaning and preparing the data for analysis.
Word2Vec: Converting text into word embeddings to capture semantic meaning.
Model Training: Training a Random Forest Classifier to classify the reviews.
Evaluation: Evaluating the model's performance using accuracy and classification metrics.
Dataset
The dataset used for this project is the IMDB Movie Reviews dataset. The dataset contains 50,000 reviews, with labels indicating whether the review is positive or negative.

You can download the dataset from Kaggle - IMDB Dataset.

Dataset Format
review: The text of the movie review.
sentiment: The sentiment label (positive or negative).
Steps
1. Data Preprocessing
The data preprocessing steps include:

Removing HTML tags from the reviews.
Converting all text to lowercase.
Removing stopwords to eliminate common words that don’t contribute to sentiment.
2. Tokenization
We tokenize the reviews using the nltk.word_tokenize function. Tokenization splits the text into individual words.

3. Word2Vec Embeddings
We use the Word2Vec model from the Gensim library to convert the reviews into word embeddings. These embeddings represent the semantic meaning of the words in the reviews.

4. Training the Model
We use a Random Forest Classifier to train the model. The model is trained on the vectorized reviews and their corresponding sentiment labels.

5. Model Evaluation
The model is evaluated using accuracy, precision, recall, and F1-score metrics.

Installation
To run the project, make sure you have the following dependencies installed:

bash
Copy
Edit
pip install pandas numpy nltk gensim scikit-learn
Additionally, you will need to download the IMDB dataset from Kaggle and place it in the same directory as the script or provide the appropriate path to the dataset.

Usage
Step 1: Download the Dataset
Download the IMDB dataset from Kaggle - IMDB Dataset.
Upload the dataset to your working directory or specify the correct path in the script.
Step 2: Preprocess the Data
Run the notebook or Python script, which will:

Read the dataset.
Preprocess the reviews (remove HTML tags, lowercase text, remove stopwords).
Tokenize the reviews and create word embeddings using Word2Vec.
Step 3: Train the Model
The script will then split the dataset into training and testing sets and train the Random Forest Classifier on the training data.

Step 4: Evaluate the Model
After training, the model will predict the sentiment on the test set, and the following evaluation metrics will be displayed:

Accuracy
Precision
Recall
F1-Score
Results
The Random Forest Classifier achieved the following performance metrics on the test set:

Accuracy: 82.38%

Classification Report:
Class	Precision	Recall	F1-Score	Support
Negative (0)	0.83	0.81	0.82	4939
Positive (1)	0.82	0.84	0.83	4978
Macro avg: 0.82 for Precision, Recall, and F1-Score.
Weighted avg: 0.82 for Precision, Recall, and F1-Score.
Contributing
If you'd like to contribute to this project, feel free to submit a pull request. Any improvements, bug fixes, or suggestions are welcome!

License
This project is licensed under the MIT License - see the LICENSE file for details.
