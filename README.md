# CRNN for Music Genre Classification

## Overview
This project implements a Convolutional Recurrent Neural Network (CRNN) for music genre classification using the GTZAN dataset. The dataset is converted into Mel-Frequency Cepstral Coefficients (MFCC) features, and audio processing techniques such as Fast Fourier Transform (FFT) and Short-Time Fourier Transform (STFT) are applied for signal segmentation. The model is trained with different segment lengths and data split ratios, achieving a best accuracy of 85%.

## Features
- **Audio Preprocessing:** FFT and STFT for feature extraction  
- **Feature Conversion:** Conversion to MFCC  
- **Model Architecture:** CRNN (Convolutional and Recurrent layers)  
- **Data Splitting:** Train, validation, and test sets with different ratios  
- **Performance:** Best accuracy of 85%  

## Usage
1. Run the preprocessing script to extract MFCC features:
   ```bash
   jupyter notebook prepocessing_audio.ipynb

2. Training the Model:
   ```bash
   jupyter notebook CRNN_model_10_Segmen.ipynb

## Evaluating the Model
Modify and run the evaluation section inside CRNN_model_10_Segmen.ipynb to test model performance on validation and test sets.

## How the Code Works
1. Preprocessing Audio Data
- The prepocessing_audio.ipynb script processes audio files by applying FFT and STFT.
- Audio files are segmented into smaller parts to create multiple training samples.
- MFCC features are extracted from each segment and stored for model training.
2. Model Training
The CRNN_model_10_Segmen.ipynb script defines and trains the CRNN model. The model consists of:
- Convolutional layers for feature extraction.
- Recurrent layers (GRU/LSTM) for sequential pattern learning.
- Fully connected layers for classification.
- The dataset is split into training, validation, and test sets.
- The model is trained using different segment lengths and split ratios to optimize performance.
3. Model Evaluation
- The trained model is evaluated on validation and test sets.
- Accuracy and loss metrics are analyzed to determine performance.
- The best model achieves 85% accuracy based on experimental results.

## Dataset
This project uses the GTZAN Genre Collection, which consists of 10 genres with 100 audio samples each. Ensure the dataset is downloaded and properly structured before running the scripts.

## Results
- The best model achieved 85% accuracy.
- Experiments were conducted with different segment lengths and data split ratios.

## Contributors
- Alfina Shafiyyah Makarim (alfina.shafiyyah.makarim@mail.ugm.ac.id)
