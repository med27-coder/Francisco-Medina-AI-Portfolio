# Lab 06 — Object Detection with Transfer Learning

## Problem Statement

Move from image classification (labeling the whole image) to object detection (locating and labeling multiple objects within an image) — using transfer learning to leverage pre-trained models instead of training from scratch.

## Approach

Used TensorFlow and TensorFlow Hub to load pre-trained object detection models and apply them to new images. Key stages:

1. **Environment Setup:** Verified GPU availability with TensorFlow; installed `tensorflow-hub` and `tensorflow-datasets`.
2. **Transfer Learning:** Loaded a pre-trained detector from TensorFlow Hub (trained on large-scale datasets like COCO or Open Images).
3. **Inference Pipeline:** Passed images through the detector to obtain bounding boxes, class labels, and confidence scores.
4. **Visualization:** Drew bounding boxes with class labels and confidence scores onto detected images using Matplotlib.
5. **Analysis:** Evaluated detection performance and compared it against training a model from scratch.

## Results

Successfully detected multiple objects within single images using a pre-trained model with no custom training required. The transfer learning approach delivered strong performance immediately, demonstrating the power of reusing learned representations.

## Key Findings

Transfer learning is one of the most practical tools in applied AI. Training object detectors from scratch requires massive datasets and compute; loading a pre-trained model collapses that to a few lines of code. Understanding bounding box format (x_min, y_min, x_max, y_max) and confidence thresholding are critical for production use.

## Technologies Used

- Python, TensorFlow, TensorFlow Hub, Matplotlib, NumPy
- Pre-trained object detection model (COCO/Open Images)
- Google Colab (GPU recommended)

## Dataset

Standard benchmark images used for detection testing. No large dataset upload — models are pre-trained; only inference images are needed.

## How to Run

Open `Lab_06_Notebook_FranciscoMedina_ITAI1378.ipynb` in [Google Colab](https://colab.research.google.com/) with GPU enabled (Runtime → Change runtime type → GPU) and run all cells in order.

## Files

| File | Description |
|---|---|
| `Lab_06_Notebook_FranciscoMedina_ITAI1378.ipynb` | Full object detection notebook |
