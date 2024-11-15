# Summaries of various emotion detection models

# LSTM Summary
lstm_summary = """
LSTM:
- Achieved 89% accuracy on the emotion detection task.
- Training process included 10 epochs with final validation accuracy of 89%.
- Model showed high precision and recall for emotions like Anger, Sadness, and Joy.
- Classification report: 
  - Anger: Precision = 0.89, Recall = 0.89, F1 = 0.89
  - Fear: Precision = 0.87, Recall = 0.81, F1 = 0.84
  - Joy: Precision = 0.94, Recall = 0.91, F1 = 0.93
  - Sadness: Precision = 0.93, Recall = 0.93, F1 = 0.93
  - Surprise: Precision = 0.60, Recall = 0.79, F1 = 0.68
"""

# GRU Summary
gru_summary = """
GRU:
- Achieved the highest accuracy of 91% for emotion detection.
- Training process included 20 epochs, with the best performance in validation at 91% accuracy.
- The GRU model demonstrated good generalization with a high F1 score across most emotions.
- Classification report:
  - Anger: Precision = 0.90, Recall = 0.92, F1 = 0.91
  - Fear: Precision = 0.88, Recall = 0.89, F1 = 0.88
  - Joy: Precision = 0.94, Recall = 0.94, F1 = 0.94
  - Sadness: Precision = 0.95, Recall = 0.94, F1 = 0.95
  - Surprise: Precision = 0.86, Recall = 0.56, F1 = 0.68
"""

# CNN Summary
cnn_summary = """
CNN:
- Achieved 89% accuracy in emotion detection with 10 epochs.
- The model performed well on emotions such as Joy and Sadness, but had lower performance for Fear and Surprise.
- Classification report:
  - Anger: Precision = 0.90, Recall = 0.86, F1 = 0.88
  - Fear: Precision = 0.79, Recall = 0.81, F1 = 0.80
  - Joy: Precision = 0.92, Recall = 0.94, F1 = 0.93
  - Sadness: Precision = 0.95, Recall = 0.91, F1 = 0.93
  - Surprise: Precision = 0.59, Recall = 0.79, F1 = 0.68
"""

# Bi-LSTM Summary
bi_lstm_summary = """
Bi-LSTM:
- Achieved 89% accuracy with a model that included 15 epochs.
- The model performed well on emotions like Sadness, Joy, and Anger, but faced difficulty with Surprise.
- Classification report:
  - Anger: Precision = 0.92, Recall = 0.81, F1 = 0.86
  - Fear: Precision = 0.84, Recall = 0.88, F1 = 0.86
  - Joy: Precision = 0.92, Recall = 0.93, F1 = 0.92
  - Sadness: Precision = 0.95, Recall = 0.92, F1 = 0.93
  - Surprise: Precision = 0.61, Recall = 0.59, F1 = 0.60
"""

# CNN+LSTM Summary
cnn_lstm_summary = """
CNN+LSTM:
- Suboptimal performance compared to other models, with the accuracy not exceeding 89%.
- The model struggled with the convergence of both the CNN and LSTM layers.
- Classification report showed mixed results with suboptimal performance on several emotions.
"""

# Best Performing Model Summary
best_model_summary = """
Best Performing Model:
- **GRU model** achieved the highest accuracy of **91%**, making it the best-performing model for emotion detection.
"""

# Output the full summary for each model
print("LSTM Model Summary:\n", lstm_summary)
print("GRU Model Summary:\n", gru_summary)
print("CNN Model Summary:\n", cnn_summary)
print("Bi-LSTM Model Summary:\n", bi_lstm_summary)
print("CNN+LSTM Model Summary:\n", cnn_lstm_summary)
print("Best Performing Model Summary:\n", best_model_summary)
