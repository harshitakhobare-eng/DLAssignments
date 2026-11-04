# Assignment 10: Deep Learning for Audio Classification with Speech-to-Text (STT) and Text-to-Speech (TTS)

## Aim
To design and implement a deep learning application for audio classification incorporating Speech-to-Text (STT) and Text-to-Speech (TTS), and evaluate its performance using suitable metrics.

## Overview
This project implements a speech command recognition system using a Convolutional Neural Network (CNN). It classifies audio commands, converts speech into text using OpenAI Whisper, and generates spoken responses using Google Text-to-Speech (gTTS).

## Dataset
- **Dataset:** Mini Speech Commands
- **Source:** TensorFlow Speech Commands Dataset
- **Selected Classes:** Yes, No, Up, Down
- **Training Samples:** 400 per class (1,600 total)
- **Validation Samples:** 100 per class (400 total)
- **Audio Duration:** 1 second
- **Sample Rate:** 16 kHz

## Technologies Used
- Python
- TensorFlow and Keras
- Librosa
- NumPy and Pandas
- Matplotlib and Seaborn
- OpenAI Whisper (Tiny)
- Google Text-to-Speech (gTTS)
- Scikit-learn

## Methodology

1. **Data Collection:** Download and load the Mini Speech Commands dataset.
2. **Audio Preprocessing:** Decode WAV files, convert audio into fixed-length waveforms, and standardize the input duration.
3. **Feature Extraction:** Generate STFT spectrograms, Log-Mel spectrograms, and MFCC representations.
4. **Model Development:** Build a CNN using convolutional, max-pooling, dense, and dropout layers.
5. **Model Training:** Train the CNN using Adam optimizer and sparse categorical cross-entropy loss.
6. **Speech-to-Text:** Use Whisper Tiny to transcribe the input audio.
7. **Text-to-Speech:** Use gTTS to generate spoken responses based on the recognized command.

## CNN Architecture
- Input Layer
- Normalization Layer
- Conv2D (32 filters)
- MaxPooling2D
- Conv2D (64 filters)
- MaxPooling2D
- Flatten Layer
- Dense Layer (64 units)
- Dropout (0.3)
- Softmax Output Layer (4 classes)

## Evaluation Metrics
The model is evaluated using:
- Accuracy
- Weighted Precision
- Weighted Recall
- Weighted F1-Score
- Macro Precision
- Macro Recall
- Macro F1-Score
- Training Time
- Confusion Matrix
- Classification Report

## Results and Visualization
The notebook includes:
- Audio waveform visualization
- STFT, Log-Mel spectrogram, and MFCC visualization
- Training and validation accuracy graphs
- Training and validation loss graphs
- Confusion matrix
- Classification report
- Whisper transcription output
- Generated TTS audio response

## How to Run
1. Open `Assn10.ipynb` in Google Colab.
2. Run the installation and import cells.
3. Download and preprocess the dataset.
4. Execute the feature extraction and CNN training cells.
5. Evaluate the model using the generated metrics.
6. Run the Whisper STT and gTTS TTS cells to test the complete application.

## Conclusion
This project demonstrates an end-to-end speech processing pipeline combining deep learning-based audio classification with Speech-to-Text and Text-to-Speech technologies. The CNN recognizes four speech commands, Whisper converts audio into text, and gTTS generates an audible response.
