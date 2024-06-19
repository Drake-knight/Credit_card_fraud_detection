# Credit Fraud Detector

## Introduction
This project aims to utilize various predictive models to detect whether a transaction is a normal payment or a fraud. The dataset used for this project has scaled features with anonymized feature names due to privacy concerns. Despite this, we can still perform an effective analysis and build robust predictive models.

## Goals
Our primary goals for this project are:
1. Understand the distribution of the provided data.
2. Create a balanced sub-dataframe of "Fraud" and "Non-Fraud" transactions using the NearMiss algorithm.
3. Determine the classifiers to use and identify the one with the highest accuracy(LogisiticRegression, KNearest, Support Vector Classifier, DecisionTreeClassifier).
4. Create a neural network and compare its accuracy to our best classifier.
5. Understand common mistakes made with imbalanced datasets.

## Outline

### I. Understanding Our Data
#### a) Gather Sense of Our Data
- Analyze the distribution and characteristics of the dataset.

### II. Preprocessing
#### a) Scaling and Distributing
- Perform necessary scaling and distribution adjustments on the data.

#### b) Splitting the Data
- Split the data into training and testing sets for model evaluation.

### III. Random UnderSampling and Oversampling
#### a) Distributing and Correlating
- Use techniques like undersampling and oversampling to balance the dataset.
- Analyze correlations between features.

#### b) Anomaly Detection
- Implement methods to detect anomalies in the data.

#### c) Dimensionality Reduction and Clustering (t-SNE)
- Apply t-SNE for dimensionality reduction and visualize data clusters.

#### d) Classifiers
- Evaluate various classifiers to identify the best-performing one.

#### e) A Deeper Look into Logistic Regression
- Conduct an in-depth analysis of logistic regression performance.

#### f) Oversampling with SMOTE
- Apply the SMOTE algorithm to handle imbalanced data through oversampling.

### IV. Testing
#### a) Testing with Logistic Regression
- Test the performance of logistic regression on the dataset.

#### b) Neural Networks Testing (Undersampling vs Oversampling)
- Compare the performance of neural networks on undersampled and oversampled datasets.

## Correcting Mistakes from Imbalanced Datasets
- Avoid testing on the oversampled or undersampled dataset directly.
- During cross-validation, oversample or undersample the training data within the cross-validation process, not before.
- Use metrics like f1-score, precision/recall score, or confusion matrix instead of accuracy score when dealing with imbalanced datasets to avoid misleading results.
