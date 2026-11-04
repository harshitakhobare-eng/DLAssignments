# 8. Implement a pre-trained BERT model for sentiment analysis or text classification on a sample dataset.

## 1. Project Overview

This project implements a pre-trained **BERT (Bidirectional Encoder Representations from Transformers)** model for sentiment analysis using the IMDb Movie Reviews dataset.

The model is fine-tuned to classify movie reviews into two categories:
- Positive (1)
- Negative (0)

## 2. Objectives

- Implement a pre-trained BERT model.
- Perform text preprocessing and tokenization.
- Fine-tune BERT for sentiment classification.
- Evaluate model performance.
- Predict sentiment for custom text inputs.

## 3. Technologies Used

- Python
- PyTorch
- Hugging Face Transformers
- Hugging Face Datasets
- NumPy
- Google Colab

## 4. Dataset

**IMDb Movie Reviews Dataset**

- 25,000 training reviews.
- 25,000 testing reviews.
- Binary sentiment labels (Positive and Negative).

For this implementation, 2,000 training samples and 500 testing samples are selected.

Dataset: [IMDb on Hugging Face](https://huggingface.co/datasets/stanfordnlp/imdb)

## 5. Model Architecture

The project uses the `bert-base-uncased` pre-trained model.

**Workflow:**

Input Text → BERT Tokenizer → Pre-trained BERT → Classification Layer → Sentiment Prediction

## 6. Model Configuration

| Parameter | Value |
|---|---|
| Model | bert-base-uncased |
| Learning Rate | 2e-5 |
| Batch Size | 8 |
| Epochs | 2 |
| Maximum Length | 128 |
| Classes | 2 |

## 7. Evaluation

The model is evaluated using:
- Accuracy
- Evaluation Loss

The evaluation metrics are generated after training.

## 8. Sample Predictions

| Input Review | Sentiment |
|---|---|
| This movie was amazing! | Positive |
| Worst film I have ever watched. | Negative |
| Excellent acting and storyline. | Positive |
| Complete waste of time. | Negative |

## 9. Applications

- Movie review analysis.
- Product review classification.
- Customer feedback analysis.
- Social media sentiment detection.
- Text classification.

## 10. Conclusion

The project demonstrates how a pre-trained BERT model can be fine-tuned for sentiment analysis using transfer learning. The model successfully classifies movie reviews as positive or negative, demonstrating the effectiveness of transformer-based models in Natural Language Processing.

## 11. How to Run

1. Open the notebook in Google Colab.
2. Enable GPU runtime (recommended).
3. Install the required dependencies.
4. Execute all cells sequentially.
5. Train and evaluate the BERT model.
6. Test custom reviews for sentiment prediction.

**Model:** BERT  
**Dataset:** IMDb Movie Reviews  
**Task:** Binary Sentiment Classification
