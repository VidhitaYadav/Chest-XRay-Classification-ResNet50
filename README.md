## Multi-Class Chest X-Ray Disease Classification using Hybrid ResNet50-CNN
 ## Overview

This project presents a Hybrid Deep Learning Model for multi-class classification of chest X-ray images. The model combines ResNet50 Transfer Learning with custom CNN layers to classify X-rays into 7 thoracic disease categories.

The goal is to assist radiologists by providing fast and automated disease predictions from chest X-ray images.

## Objectives

Classify chest X-ray images into multiple disease categories

Improve accuracy using transfer learning + fine-tuning

Handle medical image complexity using deep learning techniques

Provide a baseline decision-support system

## Diseases Classified

Atelectasis

Cardiomegaly

Emphysema

Lung Hernia

Normal

Pneumonia

Tuberculosis

## Model Architecture

The model consists of 8 layers:

Input Layer (224 × 224 × 3)

Image Preprocessing Layer (Resize, Normalize, Augmentation)

ResNet50 Backbone (Pretrained)

Global Average Pooling

Batch Normalization

Dense Layer (256 neurons)

Dropout Layer

Output Layer (Softmax – 7 classes)

## Training Strategy
Phase 1: Feature Extraction

ResNet50 layers frozen

Model trained on extracted features

Phase 2: Fine-Tuning

Last 40 layers of ResNet50 unfrozen

Model retrained to learn domain-specific features

Optimizer & Loss

Optimizer: Adam

Loss Function: Sparse Categorical Crossentropy

Callbacks Used

ModelCheckpoint

EarlyStopping

ReduceLROnPlateau

## Performance

Test Accuracy: 79.59%

Strong performance on:

Atelectasis

Cardiomegaly

Hernia

Confusion observed between:

Pneumonia

Tuberculosis

Normal

## Evaluation Metrics

Accuracy

Confusion Matrix

Precision

Recall

F1-Score

## Dataset

Chest X-ray dataset collected from Kaggle

Multi-class dataset with 7 categories

Includes preprocessing and augmentation

## Preprocessing Techniques

Image Resizing (224 × 224)

Normalization

Data Augmentation:

Flipping

Rotation

Blur

Grayscale conversion

## Limitations

Limited and imbalanced dataset

Similar visual patterns between diseases

No use of patient metadata

No lung segmentation applied

Not ready for real clinical deployment

## Future Scope

Use larger and balanced datasets

Apply advanced preprocessing (CLAHE, segmentation)

Implement Explainable AI (Grad-CAM)

Try advanced architectures (EfficientNet, Vision Transformers)

Build a web app for real-time predictions

Extend to multi-label classification

## Technologies Used

Python

TensorFlow / Keras

NumPy

Matplotlib

Seaborn

Scikit-learn

## Output

Confusion Matrix Visualization

Classification Report

Disease Predictions

## Conclusion

This project demonstrates that a hybrid ResNet50-CNN architecture can effectively classify chest X-ray diseases. It highlights the potential of deep learning in medical image analysis, especially in resource-limited environments.
