README.md

# CIFAR10 Neural Network Model using Keras

This repository contains a neural network model designed with Keras for image classification using the CIFAR10 dataset. The model utilizes the CIFAR10 dataset, which consists of 60,000 32x32 color images in 10 classes, with 6,000 images per class.

## Model Architecture

The neural network model is built using the Keras library. It has the following architecture:

- Input layer: 3072 nodes (32x32x3) representing the flattened image pixels.
- Hidden layers:
  - Dense layer with 128 units and ReLU activation function.
  - Dense layer with 64 units and ReLU activation function.
  - Dense layer with 15 units and ReLU activation function.
- Output layer: Dense layer with 10 units (corresponding to the 10 classes in CIFAR10) and softmax activation function.

The model uses various optimization techniques, such as dropout and Adam optimizer, to improve performance and prevent overfitting.

## Dataset

The CIFAR10 dataset is used as the data source. It is loaded using the `cifar10.load_data()` function from the Keras datasets module. The dataset is divided into training and testing sets, with 50,000 images for training and 10,000 images for testing.

## Model Training and Evaluation

The model is trained using the training set and evaluated using the testing set. The training process involves fitting the model to the training data for a specified number of epochs. The training progress is visualized using TensorBoard, and the model with the best performance is saved.

After training, the model is evaluated using the testing set to calculate the test loss and accuracy. Additionally, a confusion matrix is generated to analyze the model's performance for each class.

