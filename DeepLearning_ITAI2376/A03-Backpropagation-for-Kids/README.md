# A03 — Backpropagation for Kids (Group Presentation)

## Overview

Group presentation explaining the core concept of backpropagation to a younger, non-technical audience — making one of deep learning's most important algorithms accessible without losing accuracy.

**Team:** Francisco Medina, Richard Rodriguez, Rida Kashan, Yoana Cook  
**Course:** ITAI-2376 Deep Learning | Prof. Patricia McManus | 02.04.2026

## What Was Covered

Six-section presentation structured around relatable analogies:

1. **How We Learn vs. How Computers Learn** — Paralleled human learning (practice → mistake → improve) with neural network training using a bike-riding analogy.
2. **Meet the Neural Network** — Explained nodes, layers (input → hidden → output), and how signals flow through the network.
3. **Making Mistakes and Measuring the Error** — Introduced the concept of loss: the computer measures *how wrong* it was, not just *that* it was wrong.
4. **Backpropagation — Sending the Error Backwards** — The baking analogy: tracing blame back through each friend (layer) to find who caused the salty cake.
5. **Fixing Mistakes Layer by Layer** — Explained gradient descent as tiny, stable weight adjustments across all connections, not random guessing.
6. **Try, Improve, Repeat** — Showed how thousands of forward-backward cycles produce a network that reaches near-perfect accuracy.

## Key Findings

The hardest part of explaining backpropagation simply is avoiding two failure modes: oversimplifying until it's wrong, or preserving accuracy until it's incomprehensible. The baking analogy and the bike-riding framing hit both goals — they convey *proportional blame assignment* and *iterative improvement* in terms any audience can grasp.

## Technologies / Concepts Covered

- Forward pass, loss calculation, backward pass
- Gradient descent, weight updates
- PyTorch conceptual model: `loss.backward()` and `optimizer.step()`

## Files

| File | Description |
|---|---|
| `A03_team02_franciscomedina_ITAI2376.pdf` | Full presentation deck (11 slides) |
