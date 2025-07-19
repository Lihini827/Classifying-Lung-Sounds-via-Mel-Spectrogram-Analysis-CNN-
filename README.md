# Classifying Lung Sounds for Respiratory Disorders via Mel-Spectrogram Analysis Using Custom CNN

This project introduces a **custom Convolutional Neural Network (CNN)** model to classify lung sounds associated with various respiratory disorders. The core idea is to convert lung sound audio recordings into **Mel-spectrograms**—2D image representations of audio data—and use CNN-based image classification techniques for accurate disease detection.

## 🩺 Project Overview

- **Goal**: Classify different types of respiratory diseases using lung sound recordings.
- **Method**: Transform audio signals into Mel-spectrograms and use a custom-designed CNN for classification.
- 

---

## 📂 Project Structure & Steps

### ✅ Step 1: Audio Preprocessing
- Performed **time-stretching** and **noise addition** to increase diversity in audio data.
- Implemented in: [`AudioPreprocessing.ipynb`]

### ✅ Step 2: Convert Preprocessed Audio to Mel-Spectrograms
- Converted lung sound files to **Mel-spectrograms**.
- Implemented in: [`preprocesstoMFCC.ipynb`]

### ✅ Step 3: Mel-Spectrogram Augmentation
- **Three augmentations**: horizontal flip, 15° rotation, and random noise  
  → Implemented in: [`Aug3MFCC.ipynb`]
  
- **Five augmentations**: above 3 + brightness and contrast change  
  → Implemented in: [`Aug5MFCC.ipynb`]

### ✅ Step 4: CNN Model for Classification
- Proposed custom CNN architecture trained on augmented Mel-spectrograms.
- Implemented in: [`3_5AugMFCCcnnModel.ipynb`]

### ✅ Step 5: Model Evaluation
- Evaluated the model using metrics and **ROC curves**.
- Achieved **~95% classification accuracy**.
- Implemented in: [`ROC95%accuracy.ipynb`]

---

## 🧠 Key Features

- Custom CNN model tailored for Mel-spectrogram inputs
- Robust preprocessing and data augmentation pipeline
- High accuracy in classifying respiratory conditions
- Easy-to-follow and modular Jupyter notebooks


---

## 📌 Requirements

- Python 3.x
- TensorFlow / Keras
- Librosa
- OpenCV
- Matplotlib, NumPy, Scikit-learn, etc.

