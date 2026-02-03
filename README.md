# Arabic Spoken Command Recognition

## Overview
This project implements an **isolated Arabic spoken command recognition system**
using classical speech processing techniques and machine learning classifiers.

The system focuses on recognizing a small set of Arabic voice commands and
demonstrates the effectiveness of **MFCC-based features** combined with
traditional machine learning models in low-resource settings.

---

## Problem Statement
Arabic speech recognition is challenging due to dialectal variation and limited
public datasets. This project targets a **small-vocabulary, isolated-command**
scenario, suitable for real-time and embedded applications.

---

## Commands Recognized
The system recognizes six Arabic commands:

- ابدأ (Start)
- اغلق (Close)
- افتح (Open)
- يسار (Left)
- يمين (Right)
- توقف (Stop)

All audio samples are recorded at **16 kHz** in WAV format.

---

## Methodology

### Audio Preprocessing
- Silence removal
- Amplitude normalization

### Feature Extraction
- 13 Mel-Frequency Cepstral Coefficients (MFCC)
- Statistical aggregation:
  - Mean
  - Standard deviation
- Final feature vector size: **26 dimensions**

### Classification Models
- k-Nearest Neighbors (KNN)
- Gaussian Mixture Models (GMM)
- Random Forest (RF)
- Linear Support Vector Machine (SVM)

---

## Evaluation
- Train/Test split: **80% / 20%**
- Feature standardization using training statistics only
- Metrics:
  - Accuracy
  - Precision
  - Recall
  - F1-score
  - Confusion matrix

---

## Key Results
- **Linear SVM achieved the best performance (~90% accuracy)**
- MFCC statistical features provide strong class separability
- Most errors occur between acoustically similar commands
- GMM underperformed due to limited data and model sensitivity

---

## Tools & Libraries
- Python
- Librosa
- NumPy
- Scikit-learn
- Matplotlib

---


---

## Key Concepts Demonstrated
- Classical speech recognition pipeline
- MFCC feature extraction
- Statistical feature representation
- Model comparison under identical conditions
- Confusion matrix–based error analysis

---


