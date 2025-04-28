CIFAR-10 Image Classification Using a Custom Neural Network
Project Overview
This project explores image classification on the CIFAR-10 dataset using a fully connected (dense) neural network built from scratch with TensorFlow.
Instead of using convolutional neural networks (CNNs), we wanted to first see how much performance a basic feedforward neural network could achieve on raw image data.

The CIFAR-10 dataset was chosen because it is a standard benchmark in computer vision with a diverse set of real-world images like animals, vehicles, and everyday objects.

The main goal is to understand:

How simple neural networks perform on complex, real-world image data.

How training behavior can be visualized and interpreted.

What the limitations are, and how the model could be improved.

About Neural Networks
A neural network is a machine learning model inspired by the human brain.
There are many types of neural networks:

Feedforward Neural Networks (like the one used here)

Convolutional Neural Networks (CNNs) for image data

Recurrent Neural Networks (RNNs) for sequential data

Transformers for NLP tasks, and many more.

In this project, we built a basic feedforward network (Dense layers only) without any convolutional operations, to clearly observe the limitations and capabilities of a simple model.

Dataset: CIFAR-10
60,000 color images, 32x32 pixels each

10 classes: airplane, automobile, bird, cat, deer, dog, frog, horse, ship, truck

50,000 images used for training, 10,000 for testing

More about CIFAR-10 here

Technologies Used
Python

TensorFlow (Keras API)

NumPy

Matplotlib

Seaborn

Scikit-learn (for evaluation metrics)

Model Architecture
Flatten Layer: Converts 32x32x3 images into a 1D vector.

Dense Layer (512 neurons): Activation = ReLU

Dense Layer (256 neurons): Activation = ReLU

Dense Layer (128 neurons): Activation = ReLU

Dense Output Layer (10 neurons): Activation = Softmax

Optimizer: Adam
Loss Function: Sparse Categorical Crossentropy
Metrics: Accuracy

Why This Setup?
No CNN Layers: We intentionally used only fully connected layers to observe how far we can go without using convolutions.

Normalized Images: Pixel values were scaled to [0, 1] range for faster and smoother training.

Dense Architecture: A deeper model with 3 hidden layers was used to increase the network’s capacity to learn.

Performance Summary

Metric	Value
Training Accuracy	~49%
Validation Accuracy	~49%
Test Accuracy	~48%
Clearly, basic dense networks struggle to fully capture complex image structures without convolutional features.

Visualizations
📈 Training vs Validation Loss Curve: Shows how the model learns during training.

📈 Training vs Validation Accuracy Curve: Measures generalization ability.

📊 Confusion Matrix: Highlights where the model makes mistakes.

🖼️ Sample Predictions: Visualizes how the model classifies unseen images.

Limitations
The model struggles to achieve high accuracy because dense layers cannot effectively capture local patterns (edges, shapes) in images.

CIFAR-10 is a challenging dataset even for simple CNNs.

Overfitting signs could appear if the model becomes too deep without proper regularization.

Future Improvements
✅ Replace dense layers with Convolutional layers (CNNs).
✅ Apply Data Augmentation (random flips, rotations, zoom).
✅ Introduce Dropout layers to prevent overfitting.
✅ Experiment with learning rate scheduling or different optimizers.

How to Run
Clone the repository.

Install dependencies:

bash
Kopyala
Düzenle
pip install tensorflow matplotlib seaborn scikit-learn
Open the Jupyter Notebook Neural Network.ipynb.

Run all cells sequentially.

Author
Beyza Ispir
