# Speech Emotion Recognition

A machine learning and deep learning project for recognizing human emotions from speech signals using audio feature extraction and classification models.

---

## Overview

This project focuses on detecting emotions from speech using both traditional machine learning algorithms and deep learning models. It analyzes audio signals and extracts relevant features to classify emotions such as happy, sad, angry, and neutral.

![Speech Emotion Recognition](https://user-images.githubusercontent.com/39909903/91180489-9fe39400-e69c-11ea-9968-9adf6741d595.jpg)

---

## Dataset

The dataset used is **RAVDESS (Ryerson Audio-Visual Database of Emotional Speech and Song)**.

* https://zenodo.org/record/1188976
* https://www.kaggle.com/uwrfkaggler/ravdess-emotional-speech-audio

### Dataset Details

* 2452 audio files
* 24 speakers (12 male, 12 female)
* 8 emotions:

  * Neutral
  * Calm
  * Happy
  * Sad
  * Angry
  * Fearful
  * Disgust
  * Surprise

---

## Approach

### Audio Preprocessing

Audio signals are processed and converted into numerical features using:

* MFCC (Mel Frequency Cepstral Coefficients)
* Chroma features
* Mel Spectrogram
* Spectral Contrast
* Tonnetz

Libraries used:

* Librosa
* SoundFile

---

### Feature Extraction

* Extracted features from each audio file
* Combined features into a single vector
* Split dataset into training and testing sets

---

## Models Used

### Machine Learning

* Support Vector Machine (SVM)
* Decision Tree
* Random Forest

### Deep Learning

* Multi-Layer Perceptron (MLP)
* Convolutional Neural Network (CNN)

---

## Observations

* Traditional ML models provided moderate performance
* MLP models showed signs of overfitting
* CNN models performed better overall
* Model performance varied significantly based on architecture

---

## Project Structure

```
Speech-Emotion-Recognition/
│── utilities.py
│── loading_data.py
│── mlp_classifier_for_SER.py
│── SER_using_ML_algorithms.py
│── notebooks/
│── README.md
```

---

## Tech Stack

* Python
* NumPy, Pandas
* Librosa, SoundFile
* Scikit-learn
* Keras / TensorFlow

---

## Future Improvements

* Improve generalization and reduce overfitting
* Experiment with advanced architectures (LSTM, Transformers)
* Hyperparameter tuning
* Deploy as a real-time application

---
