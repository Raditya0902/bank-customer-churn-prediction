# Binary Classification Model Comparison

This repository contains Python code for building and evaluating neural network models for binary classification using three different techniques: normal approach, undersampling, and SMOTE.

## Introduction

In many real-world scenarios, especially in the financial and medical domains, datasets used for classification tasks are often imbalanced, meaning that one class significantly outnumbers the other. Imbalanced datasets can lead to biased models that favor the majority class and perform poorly on the minority class. To address this issue, several techniques have been developed, including undersampling and oversampling methods like SMOTE.

## Dataset

The dataset used in this project is the "Churn_Modelling.csv" dataset, which contains information about bank customers and whether they exited the bank (churned) or not. It includes features such as credit score, age, tenure, balance, and more.

## Techniques Used

1. **Normal Approach**: The dataset is split into training and testing sets without any adjustments for class imbalance.

2. **Undersampling**: Random undersampling is applied to the majority class (class 0) to create a balanced dataset.

3. **SMOTE (Synthetic Minority Over-sampling Technique)**: Synthetic samples are generated for the minority class (class 1) using SMOTE to balance the dataset.

## Neural Network Architecture

All models use a simple neural network architecture with the following layers:

1. Input layer with 11 neurons (input shape).
2. One hidden layer with 9 neurons and ReLU activation function.
3. Another hidden layer with 6 neurons and ReLU activation function.
4. Output layer with 1 neuron and sigmoid activation function.

## Evaluation Metrics

The models are evaluated using the following classification metrics:

- Accuracy
- Precision
- Recall
- F1-score

## Results

The performance of each model is compared based on these evaluation metrics. Additionally, confusion matrices are provided to visualize the model's predictions.

## Usage

To run the code:

1. Clone this repository to your local machine.
2. Make sure you have Python installed along with the required dependencies (Pandas, Matplotlib, NumPy, Scikit-learn, TensorFlow, and imbalanced-learn).
3. Run the Jupyter Notebook "bank-customer-churn.ipynb".

## Conclusion

The results of this project demonstrate the effectiveness of different techniques for handling class imbalance in binary classification tasks. By comparing the performance of the normal approach, undersampling, and SMOTE, we can determine the most suitable technique for our specific dataset and problem.
