# Complete NLP Pipeline: Preprocessing, Feature Engineering, Word2Vec, Similarity, Classification & Clustering
This project demonstrates the implementation of a complete Natural Language Processing (NLP) pipeline using Python, NLTK, Scikit-learn, and Gensim. It covers text preprocessing, feature engineering, similarity measurement, supervised learning, and unsupervised clustering on textual data.

Objective

To perform end-to-end NLP tasks including text preprocessing, feature extraction, sentence similarity, text classification, and clustering. The project also highlights the importance of POS tagging in lemmatization and the role of different techniques in transforming text into meaningful numerical representations.

Input Data

Two paragraphs containing multiple punctuation marks such as:

Period (.)
Comma (,)
Colon (:)
Semicolon (;)
Exclamation (!)
Question mark (?)
Quotation marks (“ ”)
Brackets { } [ ]

These punctuation marks are removed during preprocessing.

Additionally, sample sentences are used for similarity, classification, and clustering tasks.

Methodology
Text Preprocessing (NLTK)
Input two paragraphs as text data
Perform tokenization using NLTK
Convert text to lowercase
Remove punctuation using isalnum()
Remove stopwords using NLTK stopword corpus
Apply stemming using PorterStemmer
Apply lemmatization without POS tagging
Apply POS tagging to tokens
Perform lemmatization with POS tagging
Compare results of both lemmatization methods
Feature Engineering
Bag of Words (BoW)
Convert text into numerical vectors based on word frequency
Implemented using CountVectorizer
TF-IDF
Convert text into weighted numerical representation based on word importance
Implemented using TfidfVectorizer
Word2Vec (Gensim)
Train Word2Vec model on the given text
Parameters used:
vector_size = 100
window = 5
min_count = 1
epochs = 100
Generate word embeddings
Compute similarity between words
Handle vocabulary mismatch using safe similarity checks
Cosine Similarity
Convert sentences into TF-IDF vectors
Compute similarity between three sentences
Identify similarity scores between related and unrelated sentences
Supervised Learning (Text Classification)
Use labeled dataset (tech vs sports)
Convert text into TF-IDF vectors
Train model using Multinomial Naive Bayes
Predict category for new input sentence
Evaluate model using accuracy
Unsupervised Learning (Clustering)
Apply K-Means clustering on text data
Group similar sentences into clusters
Analyze clustering results
Technologies Used
Python
NLTK (Natural Language Toolkit)
Scikit-learn
Gensim
NumPy
Jupyter Notebook
Output
Tokenized text
Cleaned tokens after punctuation removal
Words after stopword removal
Stemmed words
Lemmatized words (with and without POS)
Comparison of lemmatization results
Bag of Words feature matrix
TF-IDF feature matrix
Word2Vec vocabulary and similarity scores
Cosine similarity matrix for sentences
Predicted class for input text
Accuracy of classification model
Cluster labels for text data
How to Run

Clone the repository

Install required libraries

pip install nltk scikit-learn gensim

Download NLTK datasets

import nltk
nltk.download('punkt')
nltk.download('stopwords')
nltk.download('wordnet')
nltk.download('averaged_perceptron_tagger')

Open the Jupyter Notebook / Colab Notebook

Run all cells

Conclusion

This project demonstrates a complete NLP workflow starting from raw text preprocessing to advanced tasks like word embeddings, similarity measurement, classification, and clustering. It shows how different NLP techniques work together to extract meaningful insights from textual data. The use of POS tagging improves lemmatization accuracy, while feature engineering and machine learning models enable effective analysis and prediction.

Author

Justin Raj S
