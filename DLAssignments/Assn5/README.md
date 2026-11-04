# 5. Implement and compare RNN, LSTM, and GRU models for sequence classification, and analyze their performance using appropriate evaluation metrics.

## 1. Project Overview

This project implements and compares three recurrent neural network architectures: **RNN, LSTM, and GRU** for sequence classification using the IMDb Movie Reviews dataset.

The models classify movie reviews into two sentiment categories:
- Positive (1)
- Negative (0)

The performance of each model is compared using different evaluation metrics and training time.

## 2. Objectives

- Implement Simple RNN, LSTM, and GRU models.
- Perform text preprocessing and sequence padding.
- Train and evaluate all three models.
- Compare their performance using evaluation metrics.
- Analyze accuracy, precision, recall, F1-score, and training time.

## 3. Technologies Used

- Python
- TensorFlow / Keras
- NumPy
- Pandas
- Matplotlib
- Seaborn
- Scikit-learn
- Google Colab

## 4. Dataset

**IMDb Movie Reviews Dataset**

- 25,000 training reviews.
- 25,000 testing reviews.
- Binary sentiment classification.
- Positive and Negative labels.

The dataset is preprocessed using tokenization and sequence padding.

## 5. Models Implemented

Three recurrent neural network architectures are implemented:

- **Simple RNN:** Processes sequential data by maintaining information from previous time steps.
- **LSTM:** Uses memory cells and gates to capture long-term dependencies.
- **GRU:** Uses update and reset gates to efficiently learn sequential patterns.

### Model Workflow

Input Text → Tokenization → Sequence Padding → RNN / LSTM / GRU → Classification → Sentiment Prediction

## 6. Model Configuration

| Parameter | Value |
|---|---|
| Vocabulary Size | 10,000 |
| Maximum Sequence Length | 200 |
| Embedding Dimension | 64 |
| Hidden Units | 64 |
| Dropout | 0.3 |
| Batch Size | 64 |
| Epochs | 5 |
| Optimizer | Adam |

## 7. Evaluation Metrics

The models are evaluated using:

- Accuracy
- Precision
- Recall
- F1-score
- Training Time
- Confusion Matrix

Training and validation accuracy/loss graphs are also generated to compare model performance.

## 8. Performance Comparison

| Model | Accuracy | Precision | Recall | F1-score |
|---|---:|---:|---:|---:|
| RNN | 67.47% | 67.52% | 67.33% | 67.43% |
| LSTM | 83.59% | 81.49% | 86.93% | 84.12% |
| GRU | 83.89% | 82.27% | 86.39% | 84.28% |

**Observations:**
- GRU achieved the highest F1-score.
- GRU achieved the highest accuracy.
- RNN had the shortest training time.
- LSTM and GRU performed better than Simple RNN.

## 9. Conclusion

The experiment demonstrates the implementation and comparison of RNN, LSTM, and GRU architectures for sequence classification.

GRU achieved the best overall performance based on F1-score, while Simple RNN had the shortest training time. The results demonstrate how advanced recurrent architectures can capture sequential dependencies more effectively than a basic RNN.

## 10. How to Run

1. Open the notebook in Google Colab.
2. Install the required dependencies.
3. Execute the notebook cells sequentially.
4. Train all three models.
5. Evaluate and compare their performance.

**Task:** Sequence Classification  
**Dataset:** IMDb Movie Reviews  
**Models:** RNN, LSTM, GRU  
**Framework:** TensorFlow / Keras
