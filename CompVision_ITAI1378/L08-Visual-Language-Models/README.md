# L08 — Visual Language Models (VLMs)

## Problem Statement

Explore Visual Language Models — AI systems that understand both images and text simultaneously — by working hands-on with CLIP and BLIP, two of the most widely used VLM architectures.

## Approach

Lab structured around three core VLM capabilities using HuggingFace Transformers:

1. **CLIP (Contrastive Language-Image Pretraining):** Learned how CLIP aligns image and text embeddings in a shared vector space. Used it for zero-shot image classification — classifying images using natural language descriptions without task-specific training.
2. **BLIP — Image Captioning:** Used `BlipForConditionalGeneration` to automatically generate natural language captions describing image content.
3. **BLIP — Visual Question Answering (VQA):** Used `BlipForQuestionAnswering` to answer free-form natural language questions about images.

VLM architecture covered — the three building blocks every VLM shares:
- **Vision Encoder** — converts images into feature embeddings
- **Language Model** — processes and generates text
- **Cross-Modal Bridge** — aligns visual and language representations

## Results

Successfully ran zero-shot classification, image captioning, and VQA using pre-trained CLIP and BLIP models. No custom training required — pre-trained weights generalized directly to new images, demonstrating the power of large-scale multimodal pretraining.

## Key Findings

VLMs close the gap between seeing and understanding. CLIP's contrastive training means it learns by comparing millions of image-text pairs — making it remarkably flexible at zero-shot tasks. BLIP extends this further by enabling generative language outputs, not just classification. These models are the foundation of modern AI assistants that can describe, reason about, and answer questions on visual content.

## Technologies Used

- Python, PyTorch, HuggingFace Transformers
- `CLIPProcessor`, `CLIPModel`
- `BlipProcessor`, `BlipForConditionalGeneration`, `BlipForQuestionAnswering`
- Pillow, Matplotlib, NumPy, Datasets
- Google Colab (GPU recommended)

## How to Run

Open `L08_Medina_Francisco_ITAI1378.ipynb` in [Google Colab](https://colab.research.google.com/) with GPU enabled (Runtime → Change runtime type → GPU) and run all cells in order.

## Files

| File | Description |
|---|---|
| `L08_Medina_Francisco_ITAI1378.ipynb` | Full VLM lab notebook — CLIP & BLIP |
