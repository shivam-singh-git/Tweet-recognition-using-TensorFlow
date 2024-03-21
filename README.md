Sentiment Analysis and Tweet Recognition using LSTM

Overview:

This project combines sentiment analysis and tweet recognition using Long Short-Term Memory (LSTM) networks, a type of recurrent neural network (RNN), implemented with TensorFlow and Keras. Sentiment analysis involves determining the sentiment or opinion expressed in a piece of text, which can be positive, negative, or neutral. Additionally, the model is capable of recognizing tweets and predicting their sentiment labels.

Project Structure:

Data:

The project utilizes three datasets: training, testing, and validation datasets, each containing textual data (tweets) and corresponding sentiment labels.
Code:

Python script for data preprocessing, model building, training, evaluation, and prediction.
Utilizes TensorFlow and Keras libraries for implementing LSTM-based neural networks.
Includes functions for visualizing model training history and confusion matrix.
Requirements:

Python 3.x
TensorFlow
Keras
NumPy
Pandas
Matplotlib
scikit-learn
Usage:

Ensure the required libraries are installed.
Place the training, testing, and validation datasets in CSV format in the project directory.
Run the provided Python script to preprocess the data, build the LSTM model, train it, and evaluate its performance.
Model predictions can be made using new tweet inputs.
Model Architecture:

The LSTM model architecture consists of an embedding layer, followed by two bidirectional LSTM layers and a dense output layer with softmax activation.
The model is compiled with sparse categorical cross-entropy loss and the Adam optimizer.
Results:

Evaluation metrics such as accuracy and loss are computed on the testing and validation datasets after training the model.
The model's performance can be visually assessed through plots of training and validation accuracy/loss.
Prediction:

The trained model can recognize tweet sentiments for new text inputs.
Predictions are made by passing the preprocessed tweets through the trained model and obtaining the class with the highest probability.
