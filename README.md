# Parkinson-Disease-Prediction

 Highlights
Converts .wav audio files to Mel-spectrogram images

Applies data augmentation techniques (time shift, noise, pitch, stretch)

Trains a ResNet50 CNN for binary classification

Implements K-Fold Cross Validation

Designed to run in Google Colab

📦 Libraries Used

Librosa – audio loading, processing, augmentation

OpenCV – resizing spectrograms

TensorFlow/Keras – deep learning model

Matplotlib – visualization

NumPy, os, random – data handling

🧪 Model Architecture

Base Model: ResNet50 (pretrained on ImageNet)

Input: 224×224 RGB Mel spectrograms

Layers:

Global Average Pooling

Dense layer with ReLU

Output: Dense layer with sigmoid for binary classification

📈 Training Approach

Processes each audio file into 5 spectrograms using augmentation

Ensures a balanced dataset of spectrograms from both classes

Uses K-Fold validation to split and train on different folds

Evaluates model performance using metrics like accuracy, loss, etc.

🧬 Dataset

This project assumes a dataset of .wav files organized into two folders:

PD_AH – for Parkinson's speech recordings

HC_AH – for healthy control recordings


