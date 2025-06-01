# Speech Emotion Recognition using MLPClassifier on RAVDESS Dataset

## Project Overview
This project builds a Speech Emotion Recognition (SER) system that classifies emotions from audio recordings using the **RAVDESS** dataset. The model uses audio feature extraction (MFCC) and a Multi-layer Perceptron (MLP) classifier from `scikit-learn` to identify emotions from speech.

---

## Dataset
**RAVDESS (Ryerson Audio-Visual Database of Emotional Speech and Song)**  
- Contains 1440 audio files recorded by 24 professional actors.
- Emotions include: Neutral, Calm, Happy, Sad, Angry, Fearful, Disgust, Surprised.
- Dataset downloaded and extracted directly in Google Colab.

---

## Features Extraction
- Audio files are processed to extract **MFCC (Mel-frequency cepstral coefficients)** features.
- Each audio sample is converted into a feature vector of 40 MFCCs.
- These features serve as input to the classifier.

---

## Model
- **Classifier**: Multi-layer Perceptron (MLPClassifier) from `sklearn`.
- Chosen for its ability to learn nonlinear mappings from audio features to emotions.
- Trained on 80% of the dataset and tested on 20%.

---

## Results
- Achieved approximately **62.85% accuracy** on the test set.
- Model performance can be improved by tuning hyperparameters or trying other classifiers.

---

## Requirements
- Python 3.x
- Libraries:
  - `numpy`
  - `librosa`
  - `scikit-learn`
  - `soundfile`

Install libraries with:
```bash
pip install numpy librosa scikit-learn soundfile
