# Comparative Study of Deep Learning Models for Sentiment Analysis

## Table of Contents
- [Model Performance Comparison](#model-performance-comparison)
  - [LSTM (Simple)](#lstm-simple)
  - [GRU](#gru)
  - [CNN](#cnn)
  - [Bi-directional LSTM](#bi-directional-lstm)
  - [CNN + LSTM](#cnn--lstm)
  - [GRU + CNN](#gru--cnn)
- [Model Performance Summary](#model-performance-summary)
- [Conclusion](#conclusion)
- [Future Work](#future-work)
- [License](#license)

## Model Performance Comparison

This repository contains the implementation and performance comparison of various deep learning models for emotion classification. The models tested include:

- **LSTM (Simple)**
- **GRU**
- **CNN**
- **Bi-directional LSTM**
- **CNN + LSTM**
- **GRU + CNN**

The aim is to predict emotions from text and evaluate the performance using metrics such as accuracy, precision, recall, and F1-score.

### LSTM (Simple)
- **Epochs:** 10
- **Final Accuracy:** 89.40%
- **Precision, Recall, F1-Score:**
    - Anger: Precision = 0.89, Recall = 0.89, F1 = 0.89
    - Fear: Precision = 0.87, Recall = 0.81, F1 = 0.84
    - Joy: Precision = 0.94, Recall = 0.91, F1 = 0.93
    - Love: Precision = 0.73, Recall = 0.82, F1 = 0.77
    - Sadness: Precision = 0.93, Recall = 0.93, F1 = 0.93
    - Surprise: Precision = 0.60, Recall = 0.79, F1 = 0.68
    - **Accuracy:** 89%

### GRU
- **Epochs:** 20
- **Final Accuracy:** 91.00%
- **Precision, Recall, F1-Score:**
    - Anger: Precision = 0.90, Recall = 0.92, F1 = 0.91
    - Fear: Precision = 0.88, Recall = 0.89, F1 = 0.88
    - Joy: Precision = 0.94, Recall = 0.94, F1 = 0.94
    - Love: Precision = 0.75, Recall = 0.85, F1 = 0.80
    - Sadness: Precision = 0.95, Recall = 0.94, F1 = 0.95
    - Surprise: Precision = 0.86, Recall = 0.56, F1 = 0.68
    - **Accuracy:** 91%

### CNN
- **Epochs:** 10
- **Final Accuracy:** 89.00%
- **Precision, Recall, F1-Score:**
    - Anger: Precision = 0.90, Recall = 0.86, F1 = 0.88
    - Fear: Precision = 0.79, Recall = 0.81, F1 = 0.80
    - Joy: Precision = 0.92, Recall = 0.94, F1 = 0.93
    - Love: Precision = 0.80, Recall = 0.77, F1 = 0.78
    - Sadness: Precision = 0.95, Recall = 0.91, F1 = 0.93
    - Surprise: Precision = 0.59, Recall = 0.79, F1 = 0.68
    - **Accuracy:** 89%

### Bi-directional LSTM
- **Epochs:** 15
- **Final Accuracy:** 89.00%
- **Precision, Recall, F1-Score:**
    - Anger: Precision = 0.92, Recall = 0.81, F1 = 0.86
    - Fear: Precision = 0.84, Recall = 0.88, F1 = 0.86
    - Joy: Precision = 0.92, Recall = 0.93, F1 = 0.92
    - Love: Precision = 0.70, Recall = 0.86, F1 = 0.77
    - Sadness: Precision = 0.95, Recall = 0.92, F1 = 0.93
    - Surprise: Precision = 0.61, Recall = 0.59, F1 = 0.60
    - **Accuracy:** 89%

### CNN + LSTM
- **Epochs:** 15
- **Final Accuracy:** 80.30%
- **Precision, Recall, F1-Score:**
    - Anger: Precision = 0.86, Recall = 0.81, F1 = 0.83
    - Fear: Precision = 0.72, Recall = 0.80, F1 = 0.76
    - Joy: Precision = 0.93, Recall = 0.94, F1 = 0.93
    - Love: Precision = 0.69, Recall = 0.78, F1 = 0.73
    - Sadness: Precision = 0.91, Recall = 0.87, F1 = 0.89
    - Surprise: Precision = 0.63, Recall = 0.72, F1 = 0.67
    - **Accuracy:** 80.30%

### GRU + CNN
- **Epochs:** 15
- **Final Accuracy:** 89.64%
- **Precision, Recall, F1-Score:**
    - Anger: Precision = 0.91, Recall = 0.90, F1 = 0.91
    - Fear: Precision = 0.88, Recall = 0.90, F1 = 0.89
    - Joy: Precision = 0.94, Recall = 0.94, F1 = 0.94
    - Love: Precision = 0.75, Recall = 0.85, F1 = 0.80
    - Sadness: Precision = 0.95, Recall = 0.94, F1 = 0.94
    - Surprise: Precision = 0.86, Recall = 0.56, F1 = 0.68
    - **Accuracy:** 89.64%

## Model Performance Summary
The **GRU** model achieved the highest accuracy of **91.00%**, followed closely by **GRU + CNN** at **91.20%**. Both of these models outperformed others in terms of accuracy and F1-score for the majority of emotion classes.

## Conclusion
- The **GRU** model achieved the highest accuracy of **91.00%**.
- **GRU + CNN** also performed well with an accuracy of **89.64%**.
- **CNN** and **Bi-directional LSTM** achieved relatively similar results, with accuracies of 89.00%.

## Future Work
- Explore the combination of more advanced models such as Transformer-based architectures.
- Fine-tune the hyperparameters for better results.
- Experiment with other types of data preprocessing techniques.

## License
This repository is licensed under the MIT License. See LICENSE for more information.
