# NEURAL NETWORKS
# Final proyect: Customer Satisfaction Prediction in the United States using Deep Learning

## 1. Introduction

This project implements a deep learning model to predict customer satisfaction scores based on demographic and behavioral features. Using the PyTorch library, we build and train a fully connected neural network (Multilayer Perceptron). The dataset used includes U.S.-based customers and is sourced from a public CSV file hosted on Google Drive.

## 2. Project Structure

The project is divided into the following main stages:

- *Library Imports*: Necessary libraries for data processing, deep learning, and visualization.
- *Dataset Loading*: The dataset is loaded directly from Google Drive using a CSV URL.
- *Data Cleaning and Preprocessing*: Filter U.S. customers, encode categorical variables, drop irrelevant columns, normalize features, and prepare the target variable.
- *Train/Test Split*: The dataset is split into 80% training and 20% test.
- *Tensor Conversion*: Data is converted into PyTorch tensors and loaders are prepared.
- *Model Definition*: A custom feedforward neural network with two hidden layers is defined.
- *Hyperparameter Tuning*: Different combinations of learning rates and momentum values are tested to select the best configuration.
- *Model Training*: The best model is trained over multiple epochs.
- *Model Evaluation*: Predictions are compared with true values using accuracy, confusion matrix, and classification report.
- *New Predictions (Extension)*: New customer profiles are used to test the trained model.

## 3. How to Run the Project

- *Environment*: Google Colab is recommended for easy execution and visualization.
- *Dependencies*: Make sure the following libraries are installed:
  - pandas
  - numpy
  - scikit-learn
  - matplotlib
  - seaborn
  - torch
- *Execution*: Simply run all the cells in the notebook in sequence.

## 4. New Customer Prediction (Extension)

This section allows testing the model on new customer data:

- Create a pandas DataFrame with the same structure as the training features.
- Ensure that all preprocessing steps (column order, scaling) are applied similarly.
- Use the trained model to predict the satisfaction category.
- The output will display the predicted satisfaction class (e.g., Low, Medium, High).

## 5. Dataset Availability

The dataset is available publicly and can be accessed from the following Google Drive link:

*Customer Dataset*: [Download CSV](https://drive.google.com/uc?id=1Xt9my-us-GRPWBzhDrbdRgi9fznXlLow)

The dataset contains fields such as Age, Income, Product Quality, Service Quality, Purchase Frequency, Gender, and Loyalty Level.

To ensure reproducibility, the dataset is sampled (5,000 rows) and filtered (USA-only) as part of the preprocessing steps.

---
