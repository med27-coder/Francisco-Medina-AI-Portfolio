# L05 — RNNs vs. Transformers vs. Vision Transformers

## Problem Statement

Compare three major deep learning architectures for sequence and image tasks side-by-side — understanding what each one does well, where each one fails, and why the field shifted from RNNs to Transformers to Vision Transformers.

## Approach

Comprehensive hands-on lab covering all three architectures:

1. **RNNs (Recurrent Neural Networks):** Built an RNN for sequence modeling. Explored vanishing gradient problems, hidden state mechanics, and the limitations of sequential processing (no parallelization).
2. **Transformers (BERT):** Loaded a pre-trained BERT model via HuggingFace Transformers. Explored the self-attention mechanism — how every token attends to every other token simultaneously — and applied BERT to a text classification task.
3. **Vision Transformers (ViT):** Applied a pre-trained ViT to image classification. Understood how ViT patches images into sequences and uses the same attention mechanism as text Transformers, unifying NLP and CV architectures.

## Results

Demonstrated the architectural evolution: RNNs work but are slow and fragile over long sequences; Transformers solve this with attention and parallelism; ViT extends the same mechanism to vision, showing that a single architecture can generalize across modalities.

## Key Findings

The shift from RNNs to Transformers wasn't just about accuracy — it was about parallelization. Training RNNs is inherently sequential; Transformers process all tokens at once. ViT's contribution was proving the attention mechanism isn't specific to language — spatial patches work just as well as word tokens.

## Technologies Used

- Python, PyTorch, HuggingFace `transformers` and `datasets`
- BERT (`bert-base-uncased`), ViT (`google/vit-base-patch16-224`)
- Matplotlib, NumPy, Scikit-learn
- Google Colab (GPU recommended)

## How to Run

Open `L05_Francisco_Medina_ITAI2376.ipynb` in [Google Colab](https://colab.research.google.com/) with GPU enabled and run all cells in order.

## Files

| File | Description |
|---|---|
| `L05_Francisco_Medina_ITAI2376.ipynb` | Full RNN / Transformer / ViT comparison notebook |
