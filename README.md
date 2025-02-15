# MFCC-Based Music Classification Project

# Overview

This project focuses on analyzing and classifying songs based on Mel-Frequency Cepstral Coefficients (MFCC). MFCC is a widely used feature extraction technique in audio signal processing, particularly in speech and music classification. The goal of this project was to categorize songs into six distinct groups using machine learning models.

# Project Motivation

The objective of this project was to analyze and categorize songs based on their audio features extracted using MFCC. By leveraging machine learning algorithms, we aimed to classify songs based on pitch, amplitude, and other key characteristics.

# Categories Considered

The dataset includes songs from the following categories:

Indian National Anthem

Marathi Bhav Geet

Marathi Lavni Songs

Hindi Film Songs by Asha Bhosale

Hindi Film Songs by Kishore Kumar

English Songs by Michael Jackson

# Methodology

The following steps were undertaken to develop and refine the classification model:

1. # Feature Extraction (MFCC Generation)

Pre-emphasis to enhance high-frequency components.

Framing and Windowing to improve temporal resolution.

Fourier Transform to represent frequency components.

Mel Scale Conversion to align with human auditory perception.

Discrete Cosine Transform (DCT) to obtain Cepstral Coefficients.

2. # Feature Engineering & Selection

Initially assumed 109 random features categorized into:

Melodic Progression

Cultural Rhythm

Vocal Ornament

Production Style

Ensemble Characteristics

Missing values in MFCC frames were filled using the mean.

Features with high correlation (>0.9) were dropped.

Feature selection using:

ANOVA F-score

Mutual Information

Random Forest

Best 10 selected features:

SCALE_KURT

SPECTRAL_FLATNESS_BAND_0

EMOTIONAL_RANGE

NOISE_LEVEL

VOCAL_TEXTURE_STD_4

VOCAL_TEXTURE_MEAN_1

PRONUNCIATION_CLARITY

CLASSICAL_VIBRATO_0

MELODIC_STRENGTH_0

TRANSITION_SKEW

3. # Model Training & Classification

We applied multiple machine learning models to classify the songs into the six categories:

Random Forest Classifier

K-Nearest Neighbors (KNN)

Support Vector Machine (SVM)

4. # Model Evaluation & Results

The trained models were evaluated using standard classification metrics.

Songs were categorized based on pitch and amplitude using the trained model.

MFCC files were also converted back into audio files (WAV) to manually validate results.

Some songs were misclassified, so manual corrections were made in an updated dataset.

# Key Findings & Learnings

MFCCs effectively capture the unique frequency characteristics of songs.

Proper data preprocessing is crucial for improving model performance.

Feature selection helped in reducing dimensionality while retaining essential information.

The combination of machine learning models helped achieve better classification accuracy.

Some challenges, such as noise in recordings and differences in microphone quality, affected feature extraction.

# Future Improvements

Improving data quality and reducing noise in recordings.

Expanding dataset size to include more diverse song categories.

Using deep learning models like CNNs or RNNs for improved accuracy.

Developing a real-time application for automatic song classification.

Exploring applications in voice cloning and music recommendation systems.

# Conclusion

This project successfully demonstrated the potential of MFCCs for classifying songs based on their audio features. By leveraging machine learning techniques, we were able to identify distinctive patterns in different genres and singers, offering valuable insights into automated music classification.
