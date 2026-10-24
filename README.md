# ML-Assignment01

## Neural Networks and Deep Learning Assignment

This repository contains my implementation of **Assignment 01 – Neural Networks and Deep Learning** for the **SE4022: Machine Learning** module, BSc (Hons) in Computer Science, Year 4, Semester 1, 2026.

The assignment focuses on implementing and training neural networks using Python and PyTorch. The project is adapted from the Berkeley CS188 machine learning project.

## Objectives

- Understand the fundamentals of neural networks and deep learning.
- Implement a binary perceptron for classification.
- Train a neural network for non-linear regression.
- Develop a neural network to classify handwritten digits using the MNIST dataset.
- Explore convolution operations and convolutional neural networks as an optional bonus task.

## Tasks Completed

### Task 1: The Perceptron

**Autograder:** Question 1 (`q1`)

Implemented the `PerceptronModel` class in [`models.py`](models.py).

Key components:

- Initialize the perceptron weight parameter.
- Calculate the dot product between input features and weights.
- Predict binary labels (`1` or `-1`).
- Train the model by updating weights for misclassified examples.

### Task 2: Non-Linear Regression

**Autograder:** Question 2 (`q2`)

Implemented the `RegressionModel` class to approximate the sine function over the interval `[-2π, 2π]`.

Key components:

- Design a neural network using linear layers.
- Apply ReLU activation functions between hidden layers.
- Calculate regression loss using Mean Squared Error (MSE).
- Train the model using gradient-based optimization.

### Task 3: Digit Classification (MNIST)

**Autograder:** Question 3 (`q3`)

Implemented the `DigitClassificationModel` class to classify handwritten digits from the MNIST dataset.

Key components:

- Process 28 × 28 pixel images represented as 784-dimensional input vectors.
- Build a neural network that produces scores for ten digit classes (0–9).
- Use cross-entropy loss for classification.
- Evaluate model performance using validation accuracy.

### Bonus Task: Convolutional Neural Networks

**Autograder:** Question 5 (`q5`)

The optional bonus task involves implementing the `Convolve` function and completing the `DigitConvolutionalModel` class.

The objective is to perform matrix convolution and use a convolutional neural network to classify handwritten digits.

## Technologies Used

- **Python** – Programming language
- **PyTorch** – Neural network implementation and training
- **NumPy** – Numerical computing
- **Matplotlib** – Data visualization
- **pytest / provided autograder** – Testing and evaluation

