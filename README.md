# Heartbeat Anomalies Classification
This project focuses on using machine learning techniques to classify heartbeat anomalies from audio recordings. By analyzing the features of these recordings, the model detects irregular heartbeats that may indicate medical conditions such as Murmur, Artifact, Extrastole, Extrahls, and Normal heartbeats.

## Overview
The aim of this project is to automate the classification of heartbeat sounds, which traditionally relies on expert knowledge. With machine learning, we can create a scalable and efficient system to assist in early diagnosis of heart conditions.

## Dataset
The dataset is sourced from Kaggle. The audio recordings are processed and analyzed using Librosa to extract various features, including:

MFCCs (Mel-frequency cepstral coefficients)
Zero Crossing Rate
Spectral Centroid
Spectral Rolloff
Chroma features
Data Preprocessing
Audio Loading: Audio files are loaded using librosa.
Feature Extraction: The key features are extracted to capture the rhythmic and spectral properties of the heartbeat sounds.


## Data Splitting:
Training set (80%)
Validation set (10%)
Testing set (10%)

## Models Used
Multiple machine learning models were evaluated, including:

RandomForestClassifier

Support Vector Classifier (SVC)

HistGradientBoostingClassifier

Voting Classifier

Stacking Classifier 

OneVsRest(logistic Regression)

## Final Model: 
Boosting + Stacking
Boosting was applied to individual models, followed by stacking. The final meta-classifier was a One-vs-Rest Logistic Regression.

### Performance (Test Set Accuracy): 78.00%

## Confusion Matrix
The confusion matrices show the performance of the final model on both the validation and test sets. See the code for detailed visualizations.

## Future Scope
Model Improvement: Explore deep learning and transfer learning.

Real-time Monitoring: Deploy the model in wearable devices for continuous heartbeat tracking.

Expanded Classification: Include more types of heart anomalies.

Clinical Collaboration: Collaborate with medical professionals for model validation.




