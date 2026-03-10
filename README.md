# Text-Pre-processing-Techniques-Using-NLTK
This project demonstrates the implementation of basic Natural Language Processing (NLP) text preprocessing techniques using Python and NLTK. Two paragraphs containing multiple punctuation marks are used as input, and several preprocessing operations are applied to clean and normalize the text for further NLP tasks.

Objective

To perform text preprocessing using NLTK by applying punctuation removal, stopword removal, stemming, and lemmatization. The project also compares lemmatization results with and without Part-of-Speech (POS) tagging to observe the difference in accuracy.

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

Methodology

Input two paragraphs as text data

Perform tokenization using NLTK

Remove punctuation marks from tokens

Remove stopwords using NLTK stopword corpus

Apply stemming using PorterStemmer

Apply lemmatization without POS tagging

Apply POS tagging for tokens

Perform lemmatization with POS tagging

Compare the results of both lemmatization methods

Technologies Used

Python

NLTK (Natural Language Toolkit)

Jupyter Notebook

Output

Tokenized words from the input text

Clean tokens after punctuation removal

Words after stopword filtering

Stemmed words

Lemmatized words without POS tagging

Lemmatized words with POS tagging

Comparison showing improved accuracy with POS-based lemmatization

How to Run

Clone the repository

Install required library

pip install nltk

Download NLTK datasets

nltk.download('punkt')
nltk.download('stopwords')
nltk.download('wordnet')
nltk.download('averaged_perceptron_tagger')

Open the Jupyter Notebook

Run all cells

Conclusion

Text preprocessing is a crucial step in Natural Language Processing pipelines. Removing punctuation and stopwords helps clean the data, while stemming and lemmatization reduce words to their base forms. Incorporating POS tagging in lemmatization improves accuracy by correctly identifying the grammatical role of words.

Author: Justin Raj S
