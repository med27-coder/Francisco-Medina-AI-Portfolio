# L08 — Visual Language Models: CLIP & BLIP

## What I Did

Explored Visual Language Models — AI systems that understand both images and text simultaneously. Used CLIP for zero-shot image classification and BLIP for image captioning and Visual Question Answering (VQA), all via HuggingFace Transformers.

## What I Learned

VLMs close the gap between seeing and understanding. CLIP aligns image and text embeddings in a shared vector space through contrastive training on millions of image-text pairs — meaning it can classify images using natural language descriptions it has never seen in that exact form. BLIP extends this to generative outputs: it can write a caption describing what's in an image or answer a free-text question about it. These models are the foundation of modern AI assistants that can describe, reason about, and respond to visual content.

## Challenges

Managing GPU memory for BLIP's generative model required careful batch sizing. Understanding the difference between CLIP's discriminative (score/rank) approach vs BLIP's generative (produce text) approach took hands-on comparison to fully internalize.

## Technologies Used

Python · PyTorch · HuggingFace Transformers (`CLIPProcessor`, `CLIPModel`, `BlipProcessor`, `BlipForConditionalGeneration`, `BlipForQuestionAnswering`) · Pillow · Matplotlib · Google Colab (GPU)

## How to Run

Open `L08_Medina_Francisco_ITAI1378.ipynb` in [Google Colab](https://colab.research.google.com/) with GPU enabled and run all cells in order.

## Files

| File | Description |
|---|---|
| `L08_Medina_Francisco_ITAI1378.ipynb` | Full VLM lab notebook |
