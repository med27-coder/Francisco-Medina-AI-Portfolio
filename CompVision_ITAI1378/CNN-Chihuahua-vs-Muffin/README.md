# CNN — Chihuahua vs. Muffin Classifier

## Problem Statement

Improve on the previous feedforward neural network workshop by building a Convolutional Neural Network (CNN) to classify images as chihuahuas or muffins — demonstrating how CNNs outperform flat networks on visual tasks by learning spatial features automatically.

## Approach

Built a CNN image classifier using PyTorch. Key pipeline stages:

1. **Dataset Setup:** Cloned the workshop repository; organized images into `train/` and `val/` folders using `ImageFolder`. Applied transforms: resize, random horizontal flip, normalize.
2. **Model Architecture:** Designed a CNN with convolutional layers, max pooling, ReLU activations, and fully connected layers for classification.
3. **Training:** Used Cross-Entropy Loss and an Adam/SGD optimizer. Trained for multiple epochs, logging training and validation loss each epoch.
4. **Evaluation:** Measured validation accuracy and compared model performance against the baseline feedforward network from the earlier workshop.

## Results

The CNN learned to distinguish chihuahuas from muffins by detecting spatial patterns (edges, textures, shapes) that the flat feedforward network could not capture. Validation loss decreased steadily across epochs, confirming the model was generalizing rather than memorizing.

## Key Findings

Convolutional layers are fundamentally better suited for image data because they preserve spatial structure. The same pixel values that look random to a flat network encode meaningful patterns — fur texture, curved edges, color gradients — that convolutions detect automatically. This lab made the theoretical advantage of CNNs tangible.

## Technologies Used

- Python, PyTorch (`nn.Module`, Conv2d, MaxPool2d, ReLU, Linear)
- `torchvision.transforms`, `ImageFolder`, `DataLoader`
- Matplotlib (loss curves, sample predictions)
- Google Colab

## Dataset

Chihuahua vs. Muffin image dataset — sourced from the [workshop repository](https://github.com/patitimoner/workshop-chihuahua-vs-muffin). Not included in this repo; clone the source repository and follow setup instructions in the notebook.

## How to Run

1. Clone the dataset repo: `git clone https://github.com/patitimoner/workshop-chihuahua-vs-muffin`
2. Open `CNN_1_Chihuahua_or_Muffin.ipynb` in [Google Colab](https://colab.research.google.com/)
3. Update the data path variable to point to the cloned folder
4. Run all cells in order

## Files

| File | Description |
|---|---|
| `CNN_1_Chihuahua_or_Muffin.ipynb` | Full CNN lab notebook |
