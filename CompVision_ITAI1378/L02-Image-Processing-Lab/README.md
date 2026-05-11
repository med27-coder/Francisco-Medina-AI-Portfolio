# L02 — Image Processing Lab: From Pixels to Perception

## Problem Statement

Build foundational computer vision skills by working directly with image data — understanding how machines "see" images as numerical arrays and how standard preprocessing operations transform raw pixels into usable inputs.

## Approach

Hands-on lab using OpenCV, NumPy, and Matplotlib in Google Colab. Tasks included loading and displaying images, applying grayscale conversion, resizing, filtering (blur, sharpen, edge detection), and channel manipulation. Both downloaded sample images and custom uploads were supported.

Key concepts practiced:
- Image as a NumPy array (height × width × channels)
- Color space conversions (BGR ↔ RGB ↔ Grayscale)
- Spatial filtering with convolution kernels
- Matplotlib visualization pipeline for CV results

## Results

Successfully applied a complete image preprocessing pipeline. Outputs included filtered and transformed images demonstrating the effect of each operation, visualized inline within the notebook.

## Key Findings

Every computer vision pipeline starts with correct image handling. Small details — like OpenCV's BGR channel order vs. Matplotlib's RGB — cause real visual bugs if ignored. Preprocessing quality directly determines how well downstream models perform.

## Technologies Used

- Python, OpenCV (`opencv-python-headless`), NumPy, Matplotlib, Pillow
- Google Colab

## Dataset

Sample images downloaded from public URLs; custom image upload also supported.

## How to Run

Open `L02_Medina_Francisco_ITAI1378.ipynb` in [Google Colab](https://colab.research.google.com/) and run all cells in order.

## Files

| File | Description |
|---|---|
| `L02_Medina_Francisco_ITAI1378.ipynb` | Full lab notebook |
