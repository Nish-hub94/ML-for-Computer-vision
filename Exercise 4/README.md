# Exercise 4 – Convolutional Neural Network (CNN) for CIFAR-10 Classification

## Overview
In this exercise, we extend the previous **dense neural network** (Exercise 3) to a **Convolutional Neural Network (CNN)** for classifying images from the **CIFAR-10 dataset**.  

The exercise focuses on:
- Implementing convolutional layers
- Using MaxPooling and BatchNormalization
- Applying L2 regularization
- Visualizing CNN weights
- Analyzing training and test accuracy

---

## Topics Covered
- Convolutional Neural Networks (Conv2D)
- MaxPooling2D layers
- BatchNormalization
- L2 regularization
- Training analysis (epochs, learning rate, accuracy)
- Visualization of convolutional kernels
- Memory usage of Dense and Conv layers

---

## Step-by-Step Instructions

1. **Prepare the notebook**
   - Make a copy of your Exercise 3 notebook (with 2 dense layers)  
     Rename it to `CIFAR10-CNN.ipynb`.
   - Upload the dataset `CIFAR10-small.zip` to the new notebook.

2. **Modify the model**
   - Import `Conv2D` from `keras.layers`.
   - Add convolutional layers after the input layer:

```python
kernel_sz = (3, 3)
y = Conv2D(filters=32, kernel_size=kernel_sz, strides=2, activation='relu', padding='same', kernel_initializer='he_normal')(x)
y = Conv2D(filters=64, kernel_size=kernel_sz, strides=2, activation='relu', padding='same', kernel_initializer='he_normal')(y)
