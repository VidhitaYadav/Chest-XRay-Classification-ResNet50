# Chest-XRay-Classification-ResNet50
A hybrid ResNet50–CNN deep learning model for multi-class chest X-ray disease classification, including preprocessing, model evaluation, and Gradio-based deployment with uncertainty estimation.
# Hybrid ResNet50–CNN for Chest X-Ray Classification

This repository contains the implementation of a hybrid ResNet50–CNN transfer learning model for multi-class chest X-ray disease classification.

## Diseases Classified
- Atelectasis
- Cardiomegaly
- Emphysema
- Lung Hernia
- Normal
- Pneumonia
- Tuberculosis

## Features
- Transfer learning using ResNet50
- Custom CNN layers for refined feature learning
- Sobel-based edge enhancement
- Class-wise performance evaluation
- Gradio-based web deployment
- Uncertainty estimation using Monte Carlo Dropout

## Dataset
Public chest X-ray datasets collected from Kaggle (dataset link to be provided).

## Deployment
A Gradio-based interactive web interface allows users to upload chest X-ray images and receive disease probability predictions with uncertainty scores.

## Disclaimer
This project is intended for academic and research purposes only and should not be used for clinical diagnosis.

