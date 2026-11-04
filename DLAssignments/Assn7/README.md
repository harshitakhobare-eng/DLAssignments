# 7. Implement transfer learning using pre-trained AlexNet, VGG16, ResNet50, and EfficientNetB0 models for image classification, and compare their performance.

## 1. Project Overview

This project implements and compares four deep learning models — **VGG16, ResNet50, EfficientNetB0, and AlexNet** — for image classification using the CIFAR-10 dataset.

The models are trained using transfer learning to classify images into 10 different categories.

## 2. Objectives

- Implement pre-trained CNN architectures.
- Apply transfer learning for image classification.
- Perform image preprocessing and normalization.
- Train and evaluate multiple models.
- Compare model performance using accuracy and loss.
- Predict classes for sample images.

## 3. Technologies Used

- Python
- TensorFlow / Keras
- NumPy
- Pandas
- Matplotlib
- Scikit-learn
- Google Colab

## 4. Dataset

**CIFAR-10 Dataset**

The dataset consists of 60,000 color images belonging to 10 classes.

- Training images: 50,000
- Testing images: 10,000
- Image size: 32 × 32 pixels
- Number of classes: 10

The images are resized to 224 × 224 pixels for compatibility with the pre-trained models.

**Classes:** Airplane, Automobile, Bird, Cat, Deer, Dog, Frog, Horse, Ship, Truck.

## 5. Models Implemented

Four CNN architectures are implemented:

- **VGG16:** Deep CNN architecture using small convolution filters.
- **ResNet50:** Uses residual connections to improve deep network training.
- **EfficientNetB0:** Provides efficient image classification with optimized network scaling.
- **AlexNet:** A traditional CNN architecture using convolutional and fully connected layers.

### Workflow

CIFAR-10 Dataset → Image Preprocessing → Transfer Learning Models → Classification → Performance Comparison

## 6. Model Configuration

| Parameter | Value |
|---|---|
| Image Size | 224 × 224 |
| Batch Size | 32 |
| Epochs | 2 |
| Optimizer | Adam |
| Learning Rate | 0.001 |
| Loss Function | Categorical Crossentropy |
| Number of Classes | 10 |

## 7. Performance Comparison

| Model | Test Accuracy |
|---|---:|
| AlexNet | 68.57% |
| VGG16 | 84.88% |
| ResNet50 | 89.50% |
| EfficientNetB0 | 89.76% |

**Best Model:** EfficientNetB0

EfficientNetB0 achieved the highest test accuracy of **89.76%** among the four models.

## 8. Evaluation

The models are evaluated using:

- Test Accuracy
- Test Loss
- Training and Validation Accuracy
- Training and Validation Loss
- Sample Image Predictions

Performance comparison graphs are generated using Matplotlib.

## 9. Conclusion

The experiment demonstrates the effectiveness of transfer learning for image classification using pre-trained CNN architectures.

Among the four models, EfficientNetB0 achieved the highest accuracy of 89.76%, followed closely by ResNet50. The results highlight the advantages of using pre-trained deep learning models for image classification tasks.

## 10. How to Run

1. Open the notebook in Google Colab.
2. Enable GPU runtime (recommended).
3. Install the required dependencies.
4. Execute the notebook cells sequentially.
5. Load and preprocess the CIFAR-10 dataset.
6. Train and evaluate all four models.
7. Compare performance and test sample predictions.

**Task:** Image Classification  
**Dataset:** CIFAR-10  
**Models:** VGG16, ResNet50, EfficientNetB0, AlexNet  
**Approach:** Transfer Learning  
**Framework:** TensorFlow / Keras
