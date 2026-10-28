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

## Project Structure

```text
ML-Assignment01/
├── models.py             # Neural network implementations
├── autograder.py         # Automated assignment tests
├── backend.py            # Assignment backend utilities
├── data/                 # Assignment datasets, including MNIST data
├── README.md             # Project documentation
├── .gitignore            # Files excluded from Git
└── input.txt             # Input data used by supporting scripts
```

The exact files and folders may differ depending on the supplied starter code. The virtual environment folder `.venv/` is intentionally excluded from GitHub.

## Installation and Setup

Follow these steps to set up and run the project on macOS or another system with Python installed.

### 1. Clone the Repository

```bash
git clone <YOUR_GITHUB_REPOSITORY_URL>
cd ML-Assignment01
```

Alternatively, download the repository and open its root directory in VS Code.

### 2. Create a Python Virtual Environment

Create an isolated Python environment using `venv`:

```bash
python3 -m venv .venv
```

### 3. Activate the Virtual Environment

On macOS or Linux:

```bash
source .venv/bin/activate
```

On Windows PowerShell:

```powershell
.venv\Scripts\Activate.ps1
```

Once activated, the terminal should display `(.venv)` before the command prompt.

### 4. Upgrade pip and Install Dependencies

```bash
python -m pip install --upgrade pip
python -m pip install numpy matplotlib torch
```

The assignment recommends using the CPU version of PyTorch to avoid hardware compatibility issues.

If NumPy compatibility errors occur, try installing a version below 2.0, such as:

```bash
python -m pip install "numpy==1.24.3"
```

### 5. Verify the Dependencies

Run the following command to check whether the required dependencies are available:

```bash
python autograder.py --check-dependencies
```

Resolve any reported dependency errors before proceeding.

## Running the Autograder

Run the provided autograder from the root directory of the repository, with the virtual environment activated.

### Task 1: Perceptron

```bash
python autograder.py -q q1
```

### Task 2: Non-Linear Regression

```bash
python autograder.py -q q2
```

### Task 3: Digit Classification

```bash
python autograder.py -q q3
```

### Bonus Task: Convolutional Neural Networks

```bash
python autograder.py -q q5
```

### Run the Complete Autograder

```bash
python autograder.py
```

Review the terminal output to identify passing tests, failed tests, and any implementation issues.

## Learning Outcomes

Through this assignment, I worked with:

- Perceptron learning and weight updates.
- Feedforward neural network architecture.
- Forward propagation and loss calculation.
- Gradient-based optimization and backpropagation.
- Regression using Mean Squared Error.
- Multi-class classification using cross-entropy loss.
- MNIST image classification and model evaluation.
- Convolution operations and CNN architecture concepts.

