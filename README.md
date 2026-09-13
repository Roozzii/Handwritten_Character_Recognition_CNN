# Handwritten Character Recognition using CNN

A complete deep learning pipeline for classifying handwritten digits using a Convolutional Neural Network (CNN) in TensorFlow/Keras, benchmarked against a classical Support Vector Machine (SVM) baseline. Developed as part of an internship project evaluation.

---

## Project Overview

This project implements an end-to-end image classification system using the MNIST dataset. It satisfies all core evaluation criteria including comparative baseline modeling, training stability analysis, visual error inspection, and performance benchmarking.

---

## Key Components & Results

* **Non-Neural Baseline:** Evaluated against an SVM classifier trained on flattened image pixels, achieving **97.28% accuracy** with a training time of $21.03$ seconds and test inference time of $30.46$ seconds.
* **CNN Architecture & Training Curves:** The custom CNN was trained over multiple epochs, showing steady convergence with loss decreasing smoothly and validation accuracy stabilizing above **98%**.
* **Confusion Matrix & Error Analysis:** The confusion matrix demonstrates strong diagonal dominance. Visual inspection of misclassified digits highlights common failure modes driven by extreme slants, unusual stroke thickness, and script ambiguity.

---

## Repository Structure

```text
├── dataset/                  # MNIST data directory
├── models/                   # Saved model weights
├── outputs/                  # Generated plots (Confusion Matrix, Training Curves)
├── src/                      # Python source scripts for training and evaluation
└── README.md
-----------
##Requirements
Python 3.8+

TensorFlow / Keras

Scikit-Learn

NumPy

Matplotlib

Seaborn
