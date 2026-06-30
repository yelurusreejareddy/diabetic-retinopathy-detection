# diabetic-retinopathy-detection

Fundus image classification for diabetic retinopathy detection using SVM and Random Forest
with wavelet-based feature extraction, SMOTE oversampling, and PCA dimensionality reduction.

## Dataset

diaretdb0 - a public fundus image benchmark with train/test splits defined by text files.

## Files Included

- diabetic_retinopathy_svm_rf.ipynb - full pipeline from feature extraction to evaluation
- presentation.pdf - project presentation slides

Note: diaretdb0 dataset not included.

## Pipeline

1. Load fundus images and convert to grayscale
2. Apply DWT (Haar wavelet), matched filter, and Gabor filter for preprocessing
3. K-means clustering to segment image regions
4. PCA to reduce features to 10 principal components
5. SMOTE to balance class distribution
6. Train and compare SVM (RBF kernel) and Random Forest (100 estimators)
7. Evaluate with accuracy, precision, recall, F1, and confusion matrix

## Stack

Python, OpenCV, PyWavelets, scikit-learn, SVM, Random Forest, SMOTE, PCA, NumPy, Matplotlib

## Results

SVM and Random Forest compared on held-out test set with classification report and accuracy bar chart.
