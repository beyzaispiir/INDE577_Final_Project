# CIFAR-10 Image Classification Using a Custom Neural Network

## Project Overview
This project explores image classification on the CIFAR-10 dataset using a fully connected (dense) neural network built with TensorFlow.  
Instead of using convolutional neural networks (CNNs), the focus here is to see how well a simple dense network can perform on real-world image data.

The main objectives are:
- Understand the behavior of basic feedforward neural networks.
- Visualize training and validation performance.
- Identify model limitations and improvement areas.

## About Neural Networks
Neural networks are machine learning models inspired by the brain.  
There are several types of networks:
- Feedforward Neural Networks (used in this project)
- Convolutional Neural Networks (CNNs)
- Recurrent Neural Networks (RNNs)
- Transformers

This project uses a simple feedforward (dense) neural network to focus on the core concepts.

## Dataset: CIFAR-10
- 60,000 color images (32x32 pixels, 3 channels)
- 10 classes: airplane, automobile, bird, cat, deer, dog, frog, horse, ship, truck
- 50,000 training images and 10,000 test images
- [Link to CIFAR-10 Dataset](https://www.cs.toronto.edu/~kriz/cifar.html)

## Technologies Used
- Python
- TensorFlow (Keras API)
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn

## Installation
- Clone the repository.
- Install required libraries:
  ```bash
  pip install tensorflow matplotlib seaborn scikit-learn

## Model Architecture
- **Input:** Flatten layer to convert 32x32x3 input into a 1D vector

### Hidden Layers
- Dense layer with 512 neurons (ReLU activation)
- Dense layer with 256 neurons (ReLU activation)
- Dense layer with 128 neurons (ReLU activation)

### Output Layer
- Dense layer with 10 neurons (Softmax activation)

### Optimizer
- Adam

### Loss Function
- Sparse Categorical Crossentropy

### Evaluation Metric
- Accuracy

## Why This Setup
- Fully connected layers are used to observe pure performance without convolution operations.
- CIFAR-10 dataset provides a realistic, challenging benchmark for simple models.
- Data normalization improves model convergence.

## Performance Summary
| Metric | Value |
|--------|-------|
| Training Accuracy | ~49% |
| Validation Accuracy | ~49% |
| Test Accuracy | ~48% |

Dense networks alone are not enough for complex image datasets like CIFAR-10, but they offer a valuable learning experience.

## Visualizations
- Training and Validation Loss Curves
- Training and Validation Accuracy Curves
- Confusion Matrix
- Sample Predictions on Test Images

## Limitations
- Dense networks struggle with spatial features in image data.
- CIFAR-10 usually requires convolutional layers for better performance.
- Limited generalization ability without more complex architectures.

## Future Improvements
- Replace dense layers with convolutional layers (CNN)
- Apply data augmentation techniques
- Introduce regularization like dropout and batch normalization
- Try different optimizers and learning rate schedules
  
