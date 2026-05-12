# L03 — Classical ML for Vision

## What I Did

Built an image classification pipeline using classical machine learning — feature extraction followed by Scikit-learn classifiers — without any neural networks. Covered the full pipeline from raw images to a trained and evaluated model.

## What I Learned

The key insight is that feature quality drives accuracy entirely in classical pipelines. Unlike CNNs that learn features automatically, classical ML forces you to decide what visual information matters — which builds real intuition about what makes images distinctive. This directly transfers to designing and debugging deep learning models later.

## Challenges

Choosing which features to extract and in what format was harder than writing the classifier code itself. The model's accuracy ceiling was determined by feature design decisions made before any training happened.

## Technologies Used

Python · OpenCV · Scikit-learn · Scikit-image · NumPy · Matplotlib · Google Colab

## How to Run

Open `L03_A_Francisco_Medina_ITAI1378.ipynb` in [Google Colab](https://colab.research.google.com/) and run all cells in order.

## Files

| File | Description |
|---|---|
| `L03_A_Francisco_Medina_ITAI1378.ipynb` | Classical ML vision notebook |
