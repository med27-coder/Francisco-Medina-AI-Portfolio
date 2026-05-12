# L06 — Object Detection with Transfer Learning

## What I Did

Moved from whole-image classification to object detection — locating and labeling multiple objects within a single image. Used SSD MobileNet V2 from TensorFlow Hub pre-trained on COCO, applied it to Pascal VOC 2007, built an IoU calculator from scratch, and ran threshold experiments to understand the precision/recall tradeoff.

## What I Learned

Object detection is fundamentally harder than classification: the model must answer "what AND where?" simultaneously. IoU (Intersection over Union) is the key metric — it measures bounding box overlap in a single number between 0 and 1. A critical debugging lesson: the COCO and VOC label numbering systems are incompatible, which silently drove precision and recall to zero until the bug was found and the comparison logic was removed.

**Key results:**
- Baseline (IoU=0.50, conf=0.50): Precision 55.61%, Recall 70.32%
- Lenient threshold (IoU=0.30): Recall jumped to 91.80%
- Strict threshold (IoU=0.70): Recall dropped to 65.57%, Precision to 40.40%

## Challenges

The COCO/VOC label mismatch was a silent bug — all metrics read zero with no error message. Tracing it required understanding that two completely different numbering systems were being compared as if they were the same. The fix was stopping class comparisons entirely and evaluating on bounding box location only.

## Technologies Used

Python · TensorFlow 2.19 · TensorFlow Hub (SSD MobileNet V2) · TensorFlow Datasets (Pascal VOC 2007) · Matplotlib · Google Colab (T4 GPU, High RAM)

## How to Run

Open `Lab_06_Notebook_FranciscoMedina_ITAI1378.ipynb` in [Google Colab](https://colab.research.google.com/) with GPU enabled and run all cells in order.

## Files

| File | Description |
|---|---|
| `Lab_06_Notebook_FranciscoMedina_ITAI1378.ipynb` | Full object detection notebook |
| `Lab_06_Journal_FranciscoMedina_ITAI1378.pdf` | 13-page lab journal with full analysis and reflection |
