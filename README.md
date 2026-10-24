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

