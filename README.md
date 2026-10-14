# BEED EEG Classification Using Machine Learning

## Overview
This project explores EEG signal classification using classical machine learning algorithms and an Artificial Neural Network (ANN). I compared multiple models and evaluated their performance on a held-out test set.

## Dataset
The working dataset contains 8,000 samples, 16 input features (`X1`–`X16`), and four target classes (0–3), with 2,000 samples per class.

Refer to the original dataset documentation for the exact meaning of each class.

## Project Workflow
- Dataset inspection and exploratory data analysis
- Train, validation, and test splitting
- Feature standardization using training data only
- Training classical machine learning models
- Building and evaluating an ANN using TensorFlow/Keras
- Comparing models using accuracy and macro F1-score
- Final evaluation using a confusion matrix and classification report

## Models Evaluated
- K-Nearest Neighbors (KNN)
- Gaussian Naive Bayes
- Support Vector Machine (SVM)
- Logistic Regression
- Artificial Neural Network (ANN)

## Results

| Model | Validation Accuracy |
|---|---:|
| KNN | 93% |
| ANN | Approximately 86% |
| SVM | 73% |
| Gaussian Naive Bayes | 72% |
| Logistic Regression | 47% |

## Best Model
KNN achieved the best performance among the evaluated models.

- **Test accuracy:** 93%
- **Test macro F1-score:** 0.93

These results apply to this dataset and experimental split.

## Technologies Used
Python, Pandas, NumPy, Matplotlib, Seaborn, Scikit-learn, TensorFlow/Keras, and Google Colab.

## Key Learnings
- Data preprocessing and feature standardization
- Training and comparing different classification models
- Evaluating precision, recall, F1-score, and confusion matrices
- Experimenting with neural networks and dropout
- Understanding why a more complex model does not always perform better

## How to Run
1. Open the notebook in Google Colab.
2. Obtain the dataset from its authorized source.
3. Update the dataset path if needed.
4. Run the notebook cells in order.

## Disclaimer
This is an educational machine learning project. The results do not establish clinical accuracy and must not be used for medical diagnosis.
