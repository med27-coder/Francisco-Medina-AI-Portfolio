# L04 — Deep Learning Data Preprocessing

## What I Did

Built preprocessing pipelines for four distinct data modalities used in deep learning: images, text, time series, and video/audio. Each modality required different handling techniques before it could be fed into a model.

## What I Learned

Preprocessing is not generic — each data type has its own structure and its own failure modes. Images need resizing, normalization, and channel ordering. Text needs tokenization, stopword removal, and lemmatization. Time series needs scaling and windowing. Video and audio need frame extraction and spectral feature conversion. Before this lab, I thought preprocessing was just cleaning obvious errors. Now I understand that it is a series of deliberate design choices that directly shapes what a model can and cannot learn.

The most surprising discovery was that video and audio are not fundamentally different from images and numerical arrays once preprocessed — video becomes a sequence of image frames, audio becomes a spectrogram matrix. Deep learning's flexibility comes from this universal representation.

## Challenges

Finding free, legally usable sample video and audio files required significant searching — most download sites required subscriptions. Understanding the memory constraints of loading full BERT on Colab's free CPU led to switching to DistilBERT, which provided the same 768-dimensional embeddings with a fraction of the memory footprint.

## Technologies Used

Python · OpenCV · NumPy · Scikit-image · NLTK · Matplotlib · Google Colab

## How to Run

Open `Lab_04_DL_Preprocessing_FM_ITAI2377.ipynb` in [Google Colab](https://colab.research.google.com/) and run all cells in order.

## Files

| File | Description |
|---|---|
| `Lab_04_DL_Preprocessing_FM_ITAI2377.ipynb` | Full preprocessing notebook |
| `L04_Journal_FranciscoMedina_ITAI2377.pdf` | Reflective journal |
