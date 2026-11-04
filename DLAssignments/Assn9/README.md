# 9. Perform image classification using a pre-trained Vision Transformer (ViT) model and compare its performance with a CNN model.

## 1. Project Overview

This project implements and compares a pre-trained **Vision Transformer (ViT)** model with a **Convolutional Neural Network (CNN)** for handwritten digit classification using the MNIST dataset.

Both models classify images into 10 categories (digits 0–9) using transfer learning.

## 2. Objectives

- Implement a pre-trained Vision Transformer model.
- Implement a pre-trained CNN model.
- Perform image preprocessing and normalization.
- Train and evaluate both models.
- Compare performance using appropriate evaluation metrics.
- Analyze accuracy, precision, recall, F1-score, and training time.

## 3. Technologies Used

- Python
- PyTorch
- Torchvision
- NumPy
- Pandas
- Matplotlib
- Seaborn
- Scikit-learn
- Google Colab

## 4. Dataset

**MNIST Handwritten Digit Dataset**

The dataset contains grayscale images of handwritten digits from 0 to 9.

- Training samples used: 10,000
- Testing samples used: 2,000
- Image size: 28 × 28 pixels
- Number of classes: 10

Images are resized to 224 × 224 pixels and converted into three-channel images for compatibility with pre-trained models.

Dataset: [MNIST](https://pytorch.org/vision/stable/generated/torchvision.datasets.MNIST.html)

## 5. Models Implemented

Two pre-trained architectures are used:

- **Vision Transformer (ViT-B/16):** Uses self-attention mechanisms to learn image representations.
- **ResNet18 (CNN):** Uses convolutional layers and residual connections to extract image features.

Both models use ImageNet pre-trained weights with modified classification layers for 10-class digit classification.

### Workflow

MNIST Dataset → Image Preprocessing → Pre-trained ViT / ResNet18 → Classification → Performance Comparison

## 6. Model Configuration

| Parameter | Value |
|---|---|
| Input Size | 224 × 224 |
| Batch Size | 32 |
| Epochs | 3 |
| Optimizer | AdamW |
| Learning Rate | 0.001 |
| Loss Function | Cross Entropy Loss |
| Number of Classes | 10 |

## 7. Performance Comparison

| Metric | ViT | CNN (ResNet18) |
|---|---:|---:|
| Accuracy | 94.15% | 89.15% |
| Precision | 94.24% | 89.45% |
| Recall | 94.15% | 89.15% |
| F1-score | 94.14% | 89.10% |
| Training Time | 374.57 sec | 73.90 sec |

**Best Model:** Vision Transformer (ViT-B/16)

ViT achieved the highest test accuracy of 94.15%, outperforming ResNet18 by 5 percentage points. However, ResNet18 required significantly less training time.

## 8. Evaluation

The models are evaluated using:

- Accuracy
- Precision
- Recall
- F1-score
- Confusion Matrix
- Training Time

Training accuracy and loss graphs, classification reports, and sample image predictions are also generated.

## 9. Conclusion

The experiment demonstrates the application of transfer learning using Vision Transformers and CNNs for image classification.

ViT achieved better classification performance than ResNet18 on the selected MNIST subset, while ResNet18 was considerably faster to train. The comparison highlights the trade-off between classification performance and computational efficiency.

## 10. How to Run

1. Open the notebook in Google Colab.
2. Enable GPU runtime (recommended).
3. Install the required dependencies.
4. Execute the notebook cells sequentially.
5. Load and preprocess the MNIST dataset.
6. Train both pre-trained models.
7. Evaluate and compare their performance.

**Task:** Image Classification  
**Dataset:** MNIST  
**Models:** ViT-B/16 and ResNet18  
**Approach:** Transfer Learning  
**Framework:** PyTorch
