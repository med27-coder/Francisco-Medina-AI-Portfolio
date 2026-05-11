# L04 — Chihuahua vs. Muffin: Reflective Journal

## Overview

Reflective journal documenting the Chihuahua vs. Muffin image classification workshop. The workshop introduced the core machine learning pipeline using PyTorch — from data preprocessing to model training and evaluation — through a memorable and engaging visual challenge.

## What Was Covered

**Model Architecture:** Built `MySkynet`, a feedforward neural network using PyTorch's `nn.Module`. The network used Linear layers, ReLU activations, and a Softmax output to produce class probabilities.

**Data Preprocessing:** Images were resized to a uniform shape, converted to tensors, and normalized. `ImageFolder` organized the dataset structure and `DataLoader` handled batched loading for efficient training.

**Training Loop:** Cross-entropy loss measured prediction error. SGD updated model weights each iteration. Training and validation loss were tracked across epochs to monitor for overfitting.

**Debugging:** Encountered a `FileNotFoundError` from an incorrect data path (fixed by properly cloning the repository), and a model instantiation error from moving the model to the device before creating the instance.

## Key Reflections

- Machine learning follows a structured pipeline: data → model → train → evaluate. Understanding each stage is non-negotiable.
- Debugging is a normal and valuable part of the process — every error was a learning moment.
- Feedforward networks have real limitations for image tasks; CNNs learn spatial features (edges, textures) that flat networks miss entirely.
- The same classification techniques used for chihuahuas and muffins are deployed in medical imaging, autonomous vehicles, and security systems.

## Technologies Discussed

- PyTorch (`nn.Module`, Linear, ReLU, Softmax, CrossEntropyLoss, SGD)
- `ImageFolder`, `DataLoader`
- Training/validation loss curves, overfitting detection

## Files

| File | Description |
|---|---|
| `L04_Francisco_Medina_ITAI_1378.pdf` | Full reflective journal |
