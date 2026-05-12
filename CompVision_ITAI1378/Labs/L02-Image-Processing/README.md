# L02 — Image Processing Fundamentals

## What I Did

Worked directly with images as numerical data using OpenCV, NumPy, and Matplotlib. Built a complete image preprocessing pipeline covering color space conversions, channel separation, pixel-level operations, filtering, histogram equalization, and geometric transformations.

## What I Learned

The biggest surprise was seeing that every image is just a 3D NumPy array (height × width × 3 channels) — numbers between 0 and 255. Once that clicked, every operation became math: brightness is addition, contrast is multiplication, blur is a weighted average of neighbors. Histogram equalization showed that you can improve image quality without adding any new information — just redistributing existing pixel intensity values across a wider range.

## Challenges

OpenCV's BGR channel order (vs. Matplotlib's RGB) caused colors to appear wrong on first display — a subtle bug with no error message. Getting the convolution kernel coordinates right for edge detection also required careful attention to the difference between row/column and x/y ordering.

## Technologies Used

Python · OpenCV · NumPy · Matplotlib · Pillow · Google Colab

## How to Run

Open `L02_Medina_Francisco_ITAI1378.ipynb` in [Google Colab](https://colab.research.google.com/) and run all cells in order.

## Files

| File | Description |
|---|---|
| `L02_Medina_Francisco_ITAI1378.ipynb` | Full image processing notebook |
| `J02_Medina_Francisco_ITAI1378.pdf` | Written reflection on image processing concepts |
