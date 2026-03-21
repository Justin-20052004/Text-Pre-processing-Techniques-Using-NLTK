# NLP Text Preprocessing, Feature Engineering, and Word2Vec
This project demonstrates the implementation of fundamental Natural Language Processing (NLP) techniques using Python, NLTK, Scikit-learn, and Gensim. It includes text preprocessing, feature engineering, and word embedding methods applied on sample text data.

Objective

To perform complete NLP preprocessing and feature engineering by applying punctuation removal, stopword removal, stemming, and lemmatization. The project also compares lemmatization results with and without Part-of-Speech (POS) tagging and implements Bag of Words, TF-IDF, and Word2Vec for text representation and similarity analysis.

Input Data

Two sample paragraphs containing various punctuation marks such as:

Period (.)
Comma (,)
Colon (:)
Semicolon (;)
Exclamation (!)
Question mark (?)
Quotation marks (“ ”)

These punctuation marks are removed during preprocessing.

Additionally, a separate paragraph (>200 words) is used for Word2Vec training.

Methodology
Text Preprocessing (NLTK)
Input two paragraphs as text data
Perform tokenization using NLTK
Remove punctuation marks from tokens
Remove stopwords using NLTK stopword corpus
Apply stemming using PorterStemmer
Apply lemmatization without POS tagging
Apply POS tagging for tokens
Perform lemmatization with POS tagging
Compare the results of both lemmatization methods
Feature Engineering
Bag of Words (BoW)
Convert text into numerical representation based on word frequency
Implemented using CountVectorizer
TF-IDF
Convert text into weighted numerical representation based on importance
Implemented using TfidfVectorizer
Word2Vec (Gensim)
Train Word2Vec model on a separate dataset (>200 words)
Parameters used:
vector_size = 100
window = 5
min_count = 1
epochs = 100
Perform similarity checks between words
Handle errors such as missing vocabulary (KeyError)
Technologies Used
Python
NLTK (Natural Language Toolkit)
Scikit-learn
Gensim
NumPy
Jupyter Notebook
Output
Tokenized words from the input text
Clean tokens after punctuation removal (using isalnum())
Words after stopword removal
Stemmed words
Lemmatized words without POS tagging
Lemmatized words with POS tagging
Comparison showing improved accuracy with POS-based lemmatization
Bag of Words feature matrix
TF-IDF feature matrix
Word2Vec embeddings
Word similarity scores
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

Text preprocessing is a crucial step in NLP pipelines. Removing punctuation and stopwords helps clean the data, while stemming and lemmatization reduce words to their base forms. Incorporating POS tagging improves lemmatization accuracy. Feature engineering techniques like Bag of Words and TF-IDF convert text into numerical form, and Word2Vec provides semantic understanding by learning word relationships. Together, these techniques form the foundation of many NLP applications.

Author

Justin Raj S
