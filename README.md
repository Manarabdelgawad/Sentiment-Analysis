# Sentiment-Analysis
This project focuses on building a deep learning model to classify text data into different categories using a Recurrent Neural Network (RNN) with an LSTM layer.
The model processes text data, tokenizes it, and trains a neural network to make predictions.

Dataset
The dataset used in this project contains labeled text data for binary classification:
Positive sentiment examples: 4472
Negative sentiment examples: 16986
Dataset link :
https://www.kaggle.com/datasets/manarabdelgawad/sentiment

Data Preprocessing steps :
Convert text to lowercase
Remove non-alphanumeric characters using regular expressions
Tokenize the text using the Keras Tokenizer
Pad the sequences to ensure uniform input length

Model Architecture:
Embedding Layer: Converts input words to dense vectors of fixed size.
SpatialDropout1D: Randomly drops some word embeddings for regularization.
LSTM Layer: Captures sequential dependencies in the data.
Dense Layer: Outputs probabilities for each class using the Softmax activation function.

Evaluation:
The model's performance is evaluated using accuracy and loss metrics on the test set.
