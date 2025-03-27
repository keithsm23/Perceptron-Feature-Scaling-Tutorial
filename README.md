# Perceptron Feature Scaling Tutorial

This repository contains the code and materials for a tutorial on how feature scaling impacts the performance of the Perceptron algorithm.

## Table of Contents
- [Overview](#overview)
- [Dataset](#dataset)
- [Code](#code)
- [How to Run](#how-to-run)
- [Results](#results)
- [References](#references)

## Overview
The Perceptron is a foundational machine learning algorithm, but its performance depends heavily on input feature scales. This tutorial explores how different feature scaling techniques (Min-Max Scaling, Standardization) affect the Perceptron's accuracy, convergence speed, and decision boundaries.

## Dataset
The dataset used in this tutorial is synthetic, simulating a binary classification problem. It contains two features:
- Feature 1: Income (range: $0–$100,000)
- Feature 2: Age (range: 18–80)

You can find the dataset in the `data/` folder or download it using the provided link.

## Code
The code is written in Python and uses libraries like NumPy, Matplotlib, and scikit-learn. The main files are:
- `perceptron.ipynb`: Jupyter Notebook with experiments and visualizations.
- `perceptron.py`: Standalone Python script (optional).

To install dependencies, run:
```bash
pip install -r requirements.txt
