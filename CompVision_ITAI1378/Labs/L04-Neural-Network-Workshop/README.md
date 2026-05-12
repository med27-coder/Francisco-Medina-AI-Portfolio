# L04 — Neural Network Workshop: Chihuahua vs. Muffin (Feedforward)

## What I Did

Built a feedforward neural network called `MySkynet` using PyTorch's `nn.Module` to classify chihuahua vs. muffin images. This was the first hands-on introduction to the full ML training pipeline: data preprocessing, model architecture, loss functions, optimization, and validation.

## What I Learned

Machine learning follows a strict pipeline — data preparation → model building → training → evaluation — and each stage matters equally. Normalization turned out to be more important than expected: keeping pixel values in a consistent range directly stabilized gradient behavior during training. Tracking validation loss alongside training loss gave early warning of overfitting before it became a problem.

## Challenges

A `FileNotFoundError` from incorrect data paths required cloning the workshop repository from scratch to restore the expected directory structure. Also encountered a runtime error from moving the model to the device before instantiating it — a subtle PyTorch object instantiation order requirement that only becomes obvious when it breaks.

## Technologies Used

Python · PyTorch (`nn.Module`, `Linear`, `ReLU`, `Softmax`, `CrossEntropyLoss`, `SGD`) · `ImageFolder` · `DataLoader` · Google Colab

## Files

| File | Description |
|---|---|
| `L04_Francisco_Medina_ITAI1378.pdf` | Full reflective journal on the NN workshop |
