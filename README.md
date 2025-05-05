# PyTorch Deep Learning Models

This repository contains foundational deep learning models implemented in PyTorch, demonstrating the evolution from linear classifiers to convolutional architectures. The goal is to build an intuitive understanding of model design, training behavior, and performance evaluation.

## 📌 Project Structure

### 🔹 1. Logistic Regression (Softmax)
A multi-class classifier using a linear layer and softmax activation, trained with cross-entropy loss.
- Dataset: MNIST
- Purpose: Establish a baseline model using gradient descent

| Metric              | Result    |
|---------------------|-----------|
| Final Train Error   | 15.17%    |
| Final Validation Error | 14.70% |

---

### 🔹 2. Fully Connected Neural Network (1 Hidden Layer)

#### 🧪 Variant: Sigmoid Activation
- Architecture: `Input -> Hidden (Sigmoid) -> Output`
- Highlights: Low training error, slightly higher generalization gap

| Metric              | Result    |
|---------------------|-----------|
| Final Train Error   | 0.40%     |
| Final Validation Error | 3.55% |
| Lowest Validation Error | 3.55% |

#### ⚡ Variant: ReLU Activation
- Architecture: `Input -> Hidden (ReLU) -> Output`
- Highlights: Faster convergence, still strong generalization

| Metric              | Result    |
|---------------------|-----------|
| Final Train Error   | 0.68%     |
| Final Validation Error | 3.70% |
| Lowest Validation Error | 3.70% |

---

### 🔹 3. Convolutional Neural Network (CNN)
A basic CNN for image classification, demonstrating spatial feature extraction with Conv2D and MaxPooling.

- Architecture: `Conv2D -> ReLU -> MaxPool -> FC -> Softmax`
- Optimized for digit recognition on image input

| Metric              | Result    |
|---------------------|-----------|
| Final Train Error   | 0.61%     |
| Final Validation Error | 1.45% |
| Lowest Validation Error | 1.45% |

---

## 🧠 Key Learnings

- PyTorch autograd and training loop implementation
- Comparison of activation functions (Sigmoid vs. ReLU)
- CNN's ability to capture spatial features and reduce error
- Effects of hidden layers and non-linearity on performance

## 📁 Folder Structure

pytorch-deep-learning-models/
├── pytorch_deep_learning_models.ipynb # Main Jupyter notebook 
├── train.txt # List of training image paths or IDs
├── test.txt # List of testing image paths or IDs
├── README.md # You're reading this!
