# Exercise 3 – Neural Network Inspection and CIFAR-10 Classification

## Overview
In this exercise, we explore the functionality of a **neural network** for image classification using the **CIFAR-10 dataset**.  
We inspect the network’s architecture, analyze training behavior, experiment with **regularization**, **activation functions**, and visualize neuron outputs.

---

## Topics Covered
- Loading and running a neural network for image classification
- Understanding network architecture (layers, input/output sizes, weight matrices)
- Dataset preparation and normalization
- Training for multiple epochs and analyzing accuracy and loss
- L2 regularization and its effect on weights
- Adding layers and changing activation functions
- Visualizing neuron outputs

---

## Step-by-Step Instructions

1. **Get the required files**
   - Upload `CIFAR10-linear.py` to a new Google Colab notebook.
   - Upload `CIFAR10-small.zip` dataset to the notebook’s file section.

2. **Extract the dataset**

```python
!unzip CIFAR10-small.zip
