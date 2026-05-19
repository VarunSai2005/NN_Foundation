# NN_Foundation

A simple **Neural Network built completely from scratch using NumPy** for handwritten digit classification.

This project demonstrates the core fundamentals of deep learning without using frameworks like TensorFlow or PyTorch.

---

## Features

- Fully connected neural network implemented from scratch
- Forward propagation
- Backpropagation
- Gradient descent optimization
- ReLU activation
- Softmax output layer
- One-hot encoding
- MNIST-style digit classification
- Validation prediction with image visualization

---

## Tech Stack

- Python
- NumPy
- Pandas
- Matplotlib

---

## Project Structure

```text
NN_Foundation/
│
├── NNfoundation.ipynb     # Main notebook
└── train.csv              # Dataset
```

---

## Dataset

The notebook expects a `train.csv` dataset containing handwritten digit images.

Dataset format:

- First column → label (`0–9`)
- Remaining 784 columns → pixel values (`28x28` image flattened)

You can use the MNIST digit dataset from Kaggle.

---

## Neural Network Architecture

```text
Input Layer      : 784 neurons
Hidden Layer     : 10 neurons (ReLU)
Output Layer     : 10 neurons (Softmax)
```

---

## Implemented Functions

### Initialization
Random weight and bias initialization.

### Forward Propagation
Computes predictions through the network.

### Activation Functions
- ReLU
- Softmax

### Backpropagation
Manual gradient computation.

### Gradient Descent
Parameter updates using learning rate optimization.

### Accuracy Evaluation
Tracks model performance during training.

---

## Training

Example training call:

```python
w1, b1, w2, b2 = gradient_descent(x_train, y_train, 0.1, 2000)
```

Output example:

```text
Iteration 100: Accuracy: 0.8421
Iteration 200: Accuracy: 0.8910
...
```

---

## Prediction & Visualization

The notebook allows testing predictions on validation images:

```python
print("Predicted :", predict(a2val))
print("Actual :", y_val[val_idx])
```

It also displays the digit image using Matplotlib.

---

## How to Run

### 1. Clone Repository

```bash
git clone https://github.com/VarunSai2005/NN_Foundation.git
cd NN_Foundation
```

### 2. Install Dependencies

```bash
pip install numpy pandas matplotlib
```

### 3. Open Notebook

```bash
jupyter notebook
```

Run:

```text
NNfoundation.ipynb
```

---

## Learning Goals

This project is intended for learning:

- Neural network fundamentals
- Matrix-based computations
- Manual backpropagation
- Deep learning basics without frameworks

---

## Future Improvements

- Add multiple hidden layers
- Implement mini-batch gradient descent
- Add dropout regularization
- Save/load trained weights
- Improve accuracy
- Convert notebook into modular Python scripts

---

## Author

Developed by Varun Sai
