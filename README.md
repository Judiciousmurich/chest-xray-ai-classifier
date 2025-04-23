




# Chest X-ray Classification: Normal vs. COVID-19 vs. Pneumonia

![image](https://github.com/user-attachments/assets/df064514-f902-4ae6-944d-81a434bbdcf5)
![image](https://github.com/user-attachments/assets/7e08493f-aaf7-4425-958b-54eaa8f285e6)
![image](https://github.com/user-attachments/assets/5c9f9b80-778e-46bf-bb47-9f396291f5cb)
![image](https://github.com/user-attachments/assets/99635937-4950-4e4d-abe8-64fe80e6de27)
![image](https://github.com/user-attachments/assets/75ed63b5-a2e8-4862-ae20-1eb6a79d688a)
## Project Overview

This project implements a deep learning model to classify chest X-ray images into three categories: Normal, COVID-19, and Pneumonia. Using a dataset sourced from Kaggle, the model achieves high accuracy in distinguishing between these conditions, potentially assisting healthcare professionals in diagnosis and triage.

## Dataset

The dataset consists of chest X-ray images divided into three categories:
- **Normal**: Healthy chest X-rays showing clear lung fields and normal anatomical structures
- **COVID-19**: X-rays displaying characteristic patterns of COVID-19 infection including bilateral ground-glass opacities and peripheral consolidations
- **Pneumonia**: X-rays showing typical non-COVID pneumonia patterns with localized consolidations

## Results

The model achieved impressive classification results:
- **Total test images**: 2,456
- **Correctly classified**: 2,345
- **Incorrectly classified**: 111
- **Overall accuracy**: 95.48%

## Sample Images

### Normal X-rays
Normal chest X-rays show clear lung fields with well-defined cardiac borders, normal vascular markings, and intact, symmetrical ribcage structures.

### COVID-19 X-rays
COVID-19 chest X-rays typically display bilateral infiltrates, patchy ground-glass opacities, and peripheral distribution of abnormalities, often with a more diffuse pattern than regular pneumonia.

### Pneumonia X-rays
Non-COVID pneumonia X-rays show more localized consolidations and infiltrates, typically affecting single lobes or segments rather than the diffuse bilateral pattern characteristic of COVID-19.

## Model Performance Visualization

The model confusion matrix demonstrates strong performance across all three classes, with most misclassifications occurring between COVID-19 and regular pneumonia cases, which share some radiographic similarities.

## Data Preprocessing

The X-ray images underwent several preprocessing steps:
1. Resizing to uniform dimensions
2. Normalization
3. Data augmentation to increase training set diversity and reduce overfitting

## Model Architecture

The classification model uses a convolutional neural network architecture with:
- Several convolutional layers for feature extraction
- Batch normalization for training stability
- Dropout layers to prevent overfitting
- Dense layers for final classification

## Future Work

Potential improvements and extensions:
- Implement explainable AI techniques to visualize important regions for classification
- Expand dataset to include more diverse cases
- Test model performance on external datasets for generalizability assessment
- Deploy as a web application for accessibility
