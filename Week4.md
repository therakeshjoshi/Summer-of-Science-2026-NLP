# Week 4: Neural Networks and PyTorch Basics


---

# Day 1 (Monday): Introduction to Neural Networks

## Topics
- Why Neural Networks?
- Limitations of Linear Models
- Biological Neuron vs Artificial Neuron
- Perceptron
- Single Layer Neural Network
- Multi-Layer Neural Networks
- Input Layer, Hidden Layer, Output Layer
- Parameters, Weights, Biases

## Mathematical Concepts
- Linear Transformation
- Weighted Sum
- Bias Term

## Practical
- Implement a Perceptron using NumPy
- Visualize decision boundaries


---

# Day 2 (Tuesday): Forward Propagation and Activation Functions

## Topics
- Forward Propagation
- Hidden Layer Computations
- Non-Linearity in Neural Networks
- Activation Functions

### Activation Functions
- Sigmoid
- Tanh
- ReLU
- Leaky ReLU
- Softmax

## Practical
- Implement each activation function in Python
- Compare outputs on sample inputs
- Build a simple forward pass from scratch


---

# Day 3 (Wednesday): Loss Functions and Backpropagation

## Topics
- What is a Loss Function?
- Regression vs Classification Losses

### Loss Functions
- Mean Squared Error (MSE)
- Mean Absolute Error (MAE)
- Binary Cross Entropy
- Categorical Cross Entropy

### Backpropagation
- Chain Rule Review
- Gradient Computation
- Weight Updates

## Practical
- Compute gradients manually
- Implement backpropagation for a tiny neural network


---

# Day 4 (Thursday): Optimization and Gradient Descent

## Topics
- Gradient Descent
- Learning Rate
- Batch Gradient Descent
- Stochastic Gradient Descent (SGD)
- Mini-Batch Gradient Descent

### Optimization Challenges
- Vanishing Gradients
- Exploding Gradients
- Local Minima
- Saddle Points

### Optimizers
- SGD
- Momentum
- Adam (Introduction)

## Practical
- Visualize gradient descent on simple functions
- Experiment with different learning rates


---

# Day 5 (Friday): Introduction to PyTorch

## Topics
- Why PyTorch?
- Installation and Setup
- Tensors
- Tensor Operations
- GPU vs CPU
- Autograd
- Computational Graphs

## Practical
- Tensor creation and manipulation
- Automatic differentiation using Autograd
- Basic matrix operations

## Hands-On
- Implement Linear Regression using PyTorch


---

# Day 6 (Saturday): Building Neural Networks in PyTorch

## Topics
- nn.Module
- nn.Linear
- nn.Sequential
- Training Loop
- Validation Loop
- Model Evaluation

### Workflow
1. Load Dataset
2. Create DataLoader
3. Define Model
4. Define Loss Function
5. Define Optimizer
6. Train Model
7. Evaluate Model

## Practical Project
- Train an MLP on:
  - MNIST Digit Classification
  - OR Iris Dataset

## Practical
- Complete Neural Network Training Pipeline

---

# Week 4 Mini Project

## Task
Build and train a Neural Network using PyTorch.

### Pipeline
1. Load Dataset
2. Data Preprocessing
3. Build Neural Network
4. Train Model
5. Evaluate Performance
6. Visualize Loss Curve


---

