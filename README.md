# Pneumonia X-Ray Classification

Comparison of seven machine learning and deep learning models for automated binary classification of chest X-rays into normal and pneumonia categories.

## Overview

This project benchmarks classical machine learning approaches (Logistic Regression, SVM, Random Forest, KNN) against deep learning architectures (a custom CNN, DenseNet-121, ResNet-50) on a combined dataset of public Kaggle chest X-ray images and supplementary hospital images from Chittagong, Bangladesh.

A key finding was diagnosing a source-distribution mismatch between the original training and test partitions, and showing that correcting it improved measured accuracy more than any subsequent model tuning.

## Results

| Model | Accuracy | Training Time (s) | Inference Time (s) |
|---|---|---|---|
| Custom CNN | 91.19% | 1141.67 | 16.73 |
| DenseNet-121 | 90.64% | 1425.44 | 29.24 |
| SVM | 90.41% | 2.90 | 1.10 |
| Logistic Regression | 88.92% | 168.10 | 0.001 |
| KNN | 88.92% | 0.04 | 0.05 |
| Random Forest | 88.21% | 263.24 | 0.08 |
| ResNet-50 | 87.42% | 2742.67 | 21.88 |

## Tools

Python, TensorFlow/Keras, scikit-learn, Pandas, NumPy, Matplotlib

## Full Report

The complete methodology, analysis, and discussion are published as a preprint on ResearchGate: [Comparative Analysis of Classical Machine Learning and Deep Learning Models for Pneumonia Detection in Chest X-Ray Images](https://www.researchgate.net/publication/414259709_Comparative_Analysis_of_Classical_Machine_Learning_and_Deep_Learning_Models_for_Pneumonia_Detection_in_Chest_X-Ray_Images)
