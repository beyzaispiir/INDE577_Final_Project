# Neural Network

Neural networks have become a key part of modern machine learning, driving advancements in areas like image recognition, speech processing, and natural language understanding. They are inspired by the biological structure of the brain, where interconnected neurons transmit information and learn from data. In machine learning, neural networks work by adjusting the weights between neurons to capture patterns hidden in complex datasets.

There are many different types of neural networks. Among the most popular are:

- **Convolutional Neural Networks (CNNs)**: specialized for processing grid-like data such as images.
- **Recurrent Neural Networks (RNNs)**: specialized for sequential data like time series or text.
- **Transformers**: using attention mechanisms, achieving state-of-the-art results in language and vision tasks.

However, in this project, we deliberately chose to use a **simple feedforward (dense) neural network** — also called a **Fully Connected Neural Network**.  
Instead of relying on convolutional operations, we built a network that connects every neuron in one layer to every neuron in the next.  
The purpose of this choice is to study the basic behavior of neural networks without adding the extra complexity of convolutional layers.  
By focusing on a dense structure, we can better understand how networks learn general patterns when given only raw pixel data.

# Dataset

We applied this approach to the **CIFAR-10 dataset**, a well-known benchmark for image classification.  
It contains 60,000 color images across 10 classes:

- airplane
- automobile
- bird
- cat
- deer
- dog
- frog
- horse
- ship
- truck

Each image has a size of **32x32 pixels** with **3 color channels** (RGB).  
Despite the small size, CIFAR-10 presents a realistic challenge because of the high variability among classes.

# Project Goals

This project explores the following key areas:

- How dense neural networks perform on real-world image data without spatial feature extraction
- How normalization improves convergence during training
- How model complexity (depth and number of neurons) impacts learning
- How to analyze model behavior through loss curves, accuracy curves, and confusion matrices

# Model Architecture
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
  
