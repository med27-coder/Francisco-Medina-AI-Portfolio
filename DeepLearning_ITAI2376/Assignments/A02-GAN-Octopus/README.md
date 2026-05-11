# A02 — Neural Network Zoo: The GAN Octopus

**Team 2:** Yoana Cook · Francisco Medina · Rida Kashan · Richard Rodriguez  
**Date:** 01.29.2026

## Problem

Present Generative Adversarial Networks (GANs) to the class as part of the Neural Network Zoo assignment — explaining their architecture, training dynamics, and real-world applications through an engaging analogy.

## Approach

10-slide presentation using the Mimic Octopus (*Thaumoctopus mimicus*) as a central analogy for the GAN adversarial game. The octopus impersonates 15+ species to fool predators — exactly like the Generator fooling the Discriminator. Covered the full GAN architecture, training cycle, and four real-world application domains.

## Key Concepts Covered

- **Architecture:** Generator ("The Forger") creates fakes from random noise; Discriminator ("The Detective") judges real vs. fake
- **Training Cycle:** Generator creates → Discriminator judges → both learn → repeat until Generator produces near-perfect fakes
- **Key Insight:** The Generator never sees real data directly — it only learns from the Discriminator's feedback
- **Applications:** AI art generation (DALL-E, Stable Diffusion), deepfakes, synthetic medical imaging, game asset generation

## Reflection Findings

Compared GANs to CNNs, RNNs, and Transformers — all share layered architecture and backpropagation, but GANs are unique in their dual-network adversarial training. Main limitations: training instability and mode collapse (the Generator finding one output that consistently fools the Discriminator instead of learning diversity).

## Files

| File | Description |
|---|---|
| `A02_Team2_ITAI2376.pdf` | Full 10-slide presentation deck |
| `A02_Team2_Reflection_ITAI2376.docx` | Written reflection comparing GAN to other NN types |
