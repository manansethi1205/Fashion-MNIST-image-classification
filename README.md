# Fashion MNIST Image Classification using PyTorch

A complete end-to-end Deep Learning project that classifies clothing images from the Fashion MNIST dataset using a fully connected neural network (MLP) implemented in PyTorch.

The project demonstrates the complete deep learning workflow including data preprocessing, custom dataset creation, model building, training, regularization, and evaluation.

---

## Project Overview

The Fashion MNIST dataset contains grayscale images of clothing items belonging to 10 different classes.

Each image:
- Size: **28 × 28 pixels**
- Grayscale
- Flattened into **784 input features**

The objective is to correctly classify each image into one of the following categories:

| Label | Class |
|--------|-------|
| 0 | T-shirt/Top |
| 1 | Trouser |
| 2 | Pullover |
| 3 | Dress |
| 4 | Coat |
| 5 | Sandal |
| 6 | Shirt |
| 7 | Sneaker |
| 8 | Bag |
| 9 | Ankle Boot |

---

## Features

- PyTorch implementation from scratch
- Custom Dataset class
- DataLoader for mini-batch training
- Multi-layer Perceptron (MLP)
- Batch Normalization
- Dropout Regularization
- SGD Optimizer
- Cross Entropy Loss
- GPU support (CUDA if available)
- Model evaluation on both training and testing datasets
- Dataset visualization using Matplotlib

---

## Tech Stack

- Python
- PyTorch
- Pandas
- NumPy
- Matplotlib
- Scikit-Learn

---

## Model Architecture

```
Input (784)

↓

Linear (784 → 128)

↓

BatchNorm

↓

ReLU

↓

Dropout (0.3)

↓

Linear (128 → 64)

↓

BatchNorm

↓

ReLU

↓

Dropout (0.3)

↓

Linear (64 → 10)

↓

Class Predictions
```

---

## Training Configuration

| Parameter | Value |
|-----------|-------|
| Optimizer | SGD |
| Learning Rate | 0.1 |
| Loss Function | CrossEntropyLoss |
| Epochs | 100 |
| Batch Size | 32 |
| Weight Decay | 1e-4 |

---

## Project Workflow

1. Load Fashion MNIST dataset
2. Visualize sample images
3. Normalize pixel values
4. Split into train and test sets
5. Create custom PyTorch Dataset
6. Create DataLoaders
7. Build MLP model
8. Train using mini-batch gradient descent
9. Evaluate model accuracy
10. Compare train and test performance

---

## Repository Structure

```
.
├── fmnist_prediction.ipynb
└── README.md
```

---

## Concepts Demonstrated

- Neural Networks
- Forward Propagation
- Backpropagation
- Mini-batch Gradient Descent
- Batch Normalization
- Dropout
- Cross Entropy Loss
- GPU Training
- Data Preprocessing
- PyTorch Dataset API
- DataLoader Pipeline
- Model Evaluation

---

## Future Improvements

- Replace MLP with a Convolutional Neural Network (CNN)
- Add learning rate scheduling
- Implement Early Stopping
- Save and load trained model checkpoints
- Plot training and validation loss curves
- Add confusion matrix and classification report
- Hyperparameter tuning

---

## Learning Outcomes

Through this project, I gained hands-on experience with:

- Building neural networks using PyTorch
- Creating custom datasets
- Efficient batch loading using DataLoaders
- Implementing regularization techniques
- Training deep learning models on GPU
- Evaluating classification models
- Structuring an end-to-end deep learning pipeline

---

## Author

**Manan Sethi**

Aspiring AI/ML Engineer passionate about Deep Learning, Computer Vision, Machine Learning, and Data Science.
