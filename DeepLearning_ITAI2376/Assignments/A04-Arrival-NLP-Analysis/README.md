# A04 — Arrival (2016): Extraterrestrial Communication as a Model for NLP Challenges

**Team 2:** Yoana Cook · Rida Kashan · Francisco Medina · Richard Rodriguez  
**Date:** 02.11.2026

## Problem

Use the film *Arrival* (2016) as a lens for examining real, unsolved challenges in Natural Language Processing — showing how Dr. Louise Banks's linguistic problem maps directly onto limitations in current NLP architectures and techniques.

## Approach

Research paper and presentation analyzing the Heptapod language system through a computational linguistics lens. Each structural property of Heptapod maps to a specific NLP challenge:

| Heptapod Feature | NLP Parallel |
|---|---|
| Non-linear, holistic glyphs (no tokens) | Failure of sequential tokenization assumptions |
| No shared vocabulary or culture | Zero-shot / few-shot grounding problem |
| Symbol–reality alignment via gesture | Multimodal alignment (CLIP-style contrastive learning) |
| "Gift" vs "weapon" ambiguity | Lexical ambiguity and semantic underspecification |
| Time-nonlinear perception | Limitations of autoregressive left-to-right models |

## Results

Arrival functions as a worst-case NLP scenario: a language with no shared tokens, no sequential order, no cultural context, and no guarantee human grammar applies. Current models (Transformers, RNNs) would fail completely because they assume sequential input. The film's "computational analogue" is a semantic hypergraph — a structure no mainstream NLP architecture currently handles natively.

## Key Findings

The most important insight: Louise doesn't translate, she *communicates* — testing hypotheses and adjusting in real time. Current LLMs are trained to predict, not to genuinely ground meaning. The gap between prediction and understanding is still wide open.

## Files

| File | Description |
|---|---|
| `A04_Team02_ITAI2376.docx` | Full research paper |
| `A04_Team02_ITAI2376.pptx` | Presentation deck |
