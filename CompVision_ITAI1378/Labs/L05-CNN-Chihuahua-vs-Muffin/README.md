# L05 — CNN Chihuahua vs. Muffin Classifier

## What I Did

Upgraded from the feedforward network in L04 to a Convolutional Neural Network using PyTorch. Applied data augmentation, Conv2D layers, MaxPooling, and a Softmax output to improve classification of chihuahuas vs. muffins. Tracked training and validation loss across epochs to monitor learning.

## What I Learned

CNNs are fundamentally better for images because they preserve spatial structure — a flat network treats every pixel as independent, while convolutions detect local patterns (edges, textures, shapes) that compose into higher-level features layer by layer. The difference in performance between the L04 feedforward network and this CNN made the theoretical advantage tangible.

## Challenges

Getting `DataLoader` batch dimensions and tensor shapes to align with the Conv2D input format required careful debugging. Knowing when to stop training — reading the validation loss curve to catch the overfitting point before it degraded generalization — was a judgment call that took several attempts.

## Technologies Used

Python · PyTorch (`Conv2d`, `MaxPool2d`, `ReLU`, `Linear`) · `ImageFolder` · `DataLoader` · Matplotlib · Google Colab

## How to Run

Open `L05_Medina_Francisco_ITAI1378.ipynb` in [Google Colab](https://colab.research.google.com/) and run all cells. The Chihuahua vs. Muffin dataset should be cloned from the workshop repository before running.

## Files

| File | Description |
|---|---|
| `L05_Medina_Francisco_ITAI1378.ipynb` | Full CNN lab notebook |
| `Lab05_CNN_Journal_FranciscoMedina_ITAI1378.docx` | Reflective journal on the CNN workshop |
