# Sentiment Analysis for Emotion Classification

This project performs sentiment analysis on text data to classify emotions into six categories: Sadness, Joy, Love, Anger, Fear, and Surprise. The model is built using various deep learning techniques, including Bidirectional LSTM, GRU, and CNN, to predict the emotion conveyed in a given text.

## Table of Contents
- [Overview](#overview)
- [Technologies Used](#technologies-used)
- [Data](#data)
- [Model Architecture](#model-architecture)
- [Training the Model](#training-the-model)
- [Evaluation](#evaluation)
- [Visualizations](#visualizations)
- [How to Run](#how-to-run)
- [License](#license)

## Overview

The project utilizes a variety of deep learning architectures to perform emotion classification. The main goal is to classify the emotion of a given text into one of the following categories:
- Sadness
- Joy
- Love
- Anger
- Fear
- Surprise

The models used in this project are Bidirectional LSTM, GRU, and CNN, all trained on a dataset of labeled tweets.

## Technologies Used

- Python
- TensorFlow
- Keras
- Scikit-learn
- Numpy
- Pandas
- Matplotlib
- Seaborn
- NLTK
- Google Colab (for training)

## Data

The dataset used for this project contains labeled emotion data from tweets. The dataset is split into three parts:
- **Training Data**: For training the models
- **Validation Data**: For tuning the hyperparameters and evaluating the model during training
- **Test Data**: For final evaluation of the model's performance

Each entry contains:
- **text**: The tweet content
- **label**: The emotion label (0 to 5)

## Model Architecture

The following models were used in the project:

1. **Bidirectional LSTM Model 1**:
   - Embedding Layer
   - Conv1D Layer
   - LSTM Layers (Bidirectional)
   - Dropout for regularization
   - Dense Layer with softmax activation for multi-class classification

2. **GRU Model**:
   - Embedding Layer
   - Bidirectional GRU Layer
   - GlobalMaxPooling Layer
   - Dense Layers with Dropout for regularization

3. **CNN Model**:
   - Embedding Layer
   - Convolutional Layers (Conv1D)
   - MaxPooling Layers
   - Dense Layer for final classification

4. **Bidirectional LSTM Model 2** (with more LSTM layers):
   - Embedding Layer
   - Bidirectional LSTM Layers
   - Dropout for regularization
   - Dense Layers for output

## Training the Model

Each model was trained using the following parameters:
- **Batch Size**: 32
- **Epochs**: Varying from 10 to 20, depending on the model
- **Optimizer**: Adam
- **Loss Function**: Sparse Categorical Cross-Entropy (for integer labels) / Categorical Cross-Entropy (for one-hot encoded labels)

The models were trained on the processed data after tokenizing the text and padding the sequences.

## Evaluation

After training, the models were evaluated on the test data using:
- **Accuracy**
- **Classification Report**: Including precision, recall, and F1-score
- **Confusion Matrix**: Visualized using Seaborn for better understanding of misclassifications

## Visualizations

- **Training and Validation Accuracy/Loss**: Plots showing the progression of training and validation accuracy/loss for each model.
- **Confusion Matrix**: A heatmap showing the confusion matrix to evaluate model performance across different classes.

## How to Run

### Prerequisites

- Python 3.x
- TensorFlow
- Pandas
- Scikit-learn
- Numpy
- Matplotlib
- Seaborn
- NLTK
- Google Colab (optional for running models on GPUs)

### Steps

1. Clone the repository:
    ```bash
    git clone https://github.com/yourusername/sentiment-analysis.git
    cd sentiment-analysis
    ```

2. Install the necessary dependencies:
    ```bash
    pip install -r requirements.txt
    ```

3. Run the sentiment analysis script to train the models:
    ```bash
    python sentiment_analysis.py
    ```

4. The models will be saved and evaluated. The results will be displayed, including accuracy, confusion matrices, and classification reports.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
