# L03 — Computer Vision with Classical Machine Learning

## Problem Statement

Build a working computer vision model using classical (non-deep-learning) machine learning techniques — demonstrating that strong results are achievable through deliberate feature engineering before introducing neural networks.

## Approach

Full pipeline from raw images to trained classifier using Scikit-learn and OpenCV. The lab covered:
- Environment setup with cloud-friendly lightweight libraries
- Image loading and preprocessing (resize, grayscale, normalization)
- Feature extraction: handcrafted descriptors that capture texture, shape, and intensity patterns
- Training classical classifiers (e.g., SVM, k-NN, Random Forest) on extracted features
- Evaluating model performance with classification metrics

## Results

Successfully trained and evaluated classical ML classifiers on image data. Results confirmed that feature quality is the primary driver of accuracy in non-deep-learning CV pipelines.

## Key Findings

Classical ML for computer vision requires domain knowledge to craft meaningful features. Unlike CNNs that learn features automatically, classical pipelines force you to understand what visual information matters for your task. This builds strong intuition that transfers directly to designing and debugging deep learning models.

## Technologies Used

- Python, OpenCV (`opencv-python-headless`), Scikit-image, Scikit-learn, NumPy, Matplotlib
- Google Colab

## How to Run

Open `L03_A_Francisco_Medina_ITAI_1378.ipynb` in [Google Colab](https://colab.research.google.com/) and run all cells in order.

## Files

| File | Description |
|---|---|
| `L03_A_Francisco_Medina_ITAI_1378.ipynb` | Full lab notebook |
