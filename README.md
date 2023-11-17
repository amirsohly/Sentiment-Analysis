# Sentiment-Analysis
This appears to be implementing a neural network model for sentiment analysis using the Translated-Digikala-Dataset.
### VISIT : https://colab.research.google.com/drive/1QeL-l_f6ShyPVC0BPJyAF0u7v3DlaI6o
## 1
The code begins by importing necessary libraries such as ssl, numpy, pandas, nltk, sklearn, and keras.
## 2
The main function serves as the entry point of the program. It calls other functions to set processing parameters, train the neural network model, and analyze the dataset.
## 3
The set_processing_parameters function defines and returns a dictionary of processing parameters, including the vocabulary size and maximum number of words.
## 4
The train_imdb_network function trains the neural network model using the Translated-Digikala-Dataset dataset. It loads the dataset, performs data preprocessing, splits the data into training and testing sets, builds the neural network architecture using Keras, compiles it with the Adam optimizer and binary cross-entropy loss, and fits the model to the training data. It returns the trained network weights.
## 5
The analyze_dataset function analyzes the dataset by loading a CSV file (TranslatedDigikalaDataset.csv), preprocessing the text data, splitting it into training and testing sets, and classifying the translated data using the trained network weights. It then evaluates the classifier's accuracy.
## 6
The preprocess_text function preprocesses the text data by removing stopwords, stemming the words, tokenizing the text, and converting it into a numeric representation using the CountVectorizer.
## 7
The classify_translated_data function creates a new neural network model with the same architecture as the trained model. It sets the weights of the layers to the trained weights and freezes those layers. It then compiles and fits the model to the translated data, and predicts the sentiment of the test data.
## 8
The evaluate_classifier function evaluates the accuracy of the classifier by comparing the true labels with the predicted labels.
## 9
The code includes a check for the __main__ module and an SSL context setup.
## 10
Finally, the main function is called to execute the program.
