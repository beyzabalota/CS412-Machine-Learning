# CS412 – Machine Learning  
## Homework 1: Understanding k-NN and the Curse of Dimensionality  
**Semester**: Spring 2024  
**Student**: Beyza Balota, 31232  
**Date**: 12.03.2024  

---

## Overview

This project focuses on two key concepts in Machine Learning:

1. **Curse of Dimensionality**  
   Analyzing how distances behave in high-dimensional spaces, using synthetic data.
2. **k-Nearest Neighbors (k-NN) Classifier**  
   Training and tuning a k-NN model on the Fashion-MNIST dataset to explore the effect of varying `k` values on accuracy.

The goal is to develop an understanding of how distance metrics, dimensionality, and hyperparameters affect learning in simple models like k-NN.

---

## Dataset Information

### 1. Synthetic Dataset
- Generated random data with increasing dimensions from 1 to 100.
- Sample size: 1,000 data points per dimension.
- Measured:
  - Average distance to all points
  - Minimum distance to the closest neighbor
  - Ratio of min/avg distance

### 2. Fashion-MNIST Dataset
- Source: [https://github.com/zalandoresearch/fashion-mnist](https://github.com/zalandoresearch/fashion-mnist)
- Description: 28×28 grayscale images of 10 clothing categories (e.g., T-shirt, sneaker, bag).
- Split:
  - Training: 60,000 samples  
  - Test: 10,000 samples
- Used in raw format from `keras.datasets.fashion_mnist`

---

## Key Sections

### Part 1: Curse of Dimensionality

- Generated random points in `d`-dimensional space.
- Measured average and minimum distances from a randomly selected point.
- Observed that as dimensionality increases:
  - **All distances become similar**
  - **Nearest neighbors become less distinguishable**
- Visualized with:
  - Error bar plots of metric values across dimensions
  - Histograms of pairwise distances

### Part 2: k-NN Classifier on Fashion-MNIST

- Normalized pixel values between [0, 1]
- Flattened each 28×28 image into a 784-dimensional vector
- Split dataset into training, validation, and test sets
- Evaluated different `k` values: `[1, 3, 7, 12, 20, 30, 50, 75, 100]`
- Chose best `k` via validation accuracy
- Evaluated final test accuracy and plotted confusion matrix

---

## Results

### Curse of Dimensionality:
- As dimensions increase:
  - Average and minimum distances increase
  - Min-to-avg distance ratio shrinks toward zero
- Visual proof of the "curse" in high-dimensional ML tasks

### k-NN Classifier:
- **Best validation accuracy** at **k=7**: `~0.854`
- **Test accuracy** with optimal k=7: `~0.854`
- Clear accuracy drop with high `k` values (e.g., k=100)
- Confusion matrix shows strong classification for certain classes (e.g., T-shirts and sneakers)

---

## Libraries Used

- `numpy`, `matplotlib.pyplot`
- `keras.datasets`
- `sklearn.model_selection`, `sklearn.neighbors`, `sklearn.metrics`

---

## Learnings

- The curse of dimensionality is a serious concern in high-dimensional feature spaces.
- k-NN performs well on low to moderate-dimensional data but is sensitive to the choice of `k`.
- Visualization is key to understanding behavior in abstract spaces.


