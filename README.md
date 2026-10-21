# Handwritten Digit Recognition Using MATLAB Perceptron

## Project Description
This project implements a simple multiclass perceptron in MATLAB to recognize digits from 0 to 9 using binary pixel patterns. Each digit is represented by a 5×7 binary matrix, where `1` represents an active pixel and `0` represents an inactive pixel.

The model is trained using predefined digit patterns and then evaluated using three different test datasets containing variations of the original patterns.

## Technologies Used
- MATLAB
- Perceptron learning algorithm
- Matrix operations
- Pattern recognition
- Data classification

## How It Works

### 1. Training Data Preparation
Ten digit patterns, representing numbers from 0 to 9, are defined as 5×7 matrices. Each matrix is converted into a 35-element column vector to serve as the input to the perceptron.

### 2. Perceptron Training
The model uses a weight matrix initialized with zeros. During training, the perceptron calculates the output scores for each digit class and selects the class with the highest score.

If the predicted class is incorrect, the weights of the correct and incorrectly predicted classes are updated using the perceptron learning rule.

**Training parameters:**
- Learning rate: `0.1`
- Maximum number of epochs: `1000`
- Input features: `35`
- Output classes: `10`

Training stops when all training patterns are classified correctly or the maximum epoch limit is reached.

### 3. Testing and Evaluation
The trained model is evaluated using three separate test datasets. Each dataset contains ten digit patterns with slight variations from the training patterns.

For each test sample, the model predicts a digit between 0 and 9. The prediction is compared with the actual digit to calculate the classification accuracy.

### 4. Accuracy Calculation
The classification accuracy is calculated using the following formula:

**Accuracy (%) = (Number of Correct Predictions / Total Test Samples) × 100**

Each test dataset contains ten samples, and the accuracy is reported separately for each dataset.

## Key Features
- Recognizes ten digit classes (0–9).
- Uses binary pixel representations.
- Implements the perceptron learning algorithm from scratch.
- Updates weights when a classification error occurs.
- Evaluates performance on three different test datasets.
- Reports the number of correct predictions and classification accuracy.

## How to Run
1. Download or clone this repository.
2. Open MATLAB.
3. Open the `.m` file containing the code.
4. Run the script.
5. Review the training status, predicted digits, and accuracy results in the Command Window.

## Learning Objectives
This project demonstrates the fundamentals of supervised learning, multiclass classification, weight updates, and model evaluation using MATLAB. It also provides practical experience with matrix operations and pattern recognition without relying on built-in machine learning training functions.

## Limitations
The model uses predefined 5×7 binary patterns rather than real handwritten digit images. Its performance depends on the similarity between the training patterns and the test samples. Since the perceptron uses a linear classification approach, it may not correctly classify every variation.
