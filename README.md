# Handwritten-Digit-Classification

# Introduction to PCA

## Overview
This document explores the use of Principal Component Analysis (PCA) in a machine learning context, specifically for image classification using a dataset of numerical representations of digits. The dataset is loaded using scikit-learn's `load_digits` function, and initial exploration is conducted to understand its structure.

## Dataset Exploration
The dataset consists of 1797 images, each represented by 64 numerical features (8x8 pixel values). The target variable represents the digit each image corresponds to (ranging from 0 to 9). After loading the data, a DataFrame is created for easier analysis.

## Preparing the Model
To train a machine learning model, the features are scaled using `StandardScaler` and the data is split into training and testing sets. A Logistic Regression model is then trained on the original dataset, and its accuracy is evaluated.

## Applying PCA
Principal Component Analysis (PCA) is employed to reduce the dimensionality of the dataset. The number of principal components is chosen based on the desired variance to be retained. The explained variance ratio and the number of components are examined. Another Logistic Regression model is trained on the reduced dataset, and its accuracy is evaluated.

## Conclusion
The document concludes with a summary table showcasing the impact of different levels of retained variance on the model's accuracy after applying PCA. This analysis provides insights into the trade-off between dimensionality reduction and model accuracy. The table indicates that as we reduce the dimensionality (and retain less variance), there is a gradual decrease in accuracy, demonstrating the importance of finding a balance between dimensionality reduction and model performance.
