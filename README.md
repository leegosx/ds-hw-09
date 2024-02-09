# Fashion MNIST Neural Network Models

## Overview

This homework includes the development and comparison of two neural network models trained on the Fashion MNIST dataset. The goal is to classify images of different fashion products into 10 categories with high accuracy. The baseline model achieves approximately 91% accuracy, and our custom models aim to match or exceed this benchmark.


### Model 1: Basic Neural Network

- **Architecture**: This model includes a flatten layer, a dense layer with 128 neurons (ReLU activation), a dropout layer (0.2), and a final dense layer for classification (Softmax activation).
- **Optimizer**: Adam
- **Loss Function**: Sparse Categorical Crossentropy
- **Metrics**: Accuracy
- **Hyperparameters**: Epochs = 10, Batch Size = 64

### Model 2: Enhanced Neural Network

- **Architecture**: Begins with a flatten layer, followed by a dense layer with 512 neurons (ReLU activation), batch normalization, dropout (0.2), another dense layer with 128 neurons (ReLU activation), batch normalization, dropout (0.2), and a final classification layer.
- **Optimizer**: Adam
- **Loss Function**: Sparse Categorical Crossentropy
- **Metrics**: Accuracy
- **Hyperparameters**: Epochs = 20, Batch Size = 32

## Dataset:
- The Fashion MNIST dataset is used, which can be loaded directly via TensorFlow/Keras:
  ```
  from tensorflow.keras.datasets import fashion_mnist
  (x_train, y_train), (x_test, y_test) = fashion_mnist.load_data()
  ```
