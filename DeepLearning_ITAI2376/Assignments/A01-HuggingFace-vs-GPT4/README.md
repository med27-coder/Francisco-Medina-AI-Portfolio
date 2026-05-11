# A01 — HuggingFace Transformers vs OpenAI GPT-4 API: A Comparative Analysis

**Team 2:** Yoana Cook · Francisco Medina · Rida Kashan · Richard Rodriguez  
**Date:** 01.26.2026

## Problem

Compare two of the most widely used platforms for deploying large language models — HuggingFace Transformers (open-source) and the OpenAI GPT-4 API (proprietary cloud) — across dimensions that matter for real deployment decisions.

## Approach

Research paper analyzing both platforms across five key dimensions: background and origin, access model, customization depth, data privacy, and ease of use. Supported by real-world application examples from healthcare (HuggingFace) and financial services (GPT-4 API).

## Results

| Dimension | HuggingFace Transformers | OpenAI GPT-4 API |
|---|---|---|
| Access | Open-source; download model weights | Cloud API; no weight access |
| Customization | Full fine-tuning, architecture modification | Limited fine-tuning only |
| Privacy | On-premise deployment possible | All data processed on OpenAI servers |
| Cost | Free for most resources | Pay-per-token; scales with usage |
| Ease of Use | Requires ML expertise (PyTorch/TF) | Minimal setup; REST API |

## Key Findings

Neither platform is universally better — the choice depends entirely on the use case. HuggingFace is the right choice when customization, privacy, or cost control matter. GPT-4 API wins when speed to deployment and raw performance are the priority. The open-source vs. closed-source tradeoff in AI mirrors the same debate in software more broadly.

## Files

| File | Description |
|---|---|
| `A01a_Team02_ITAI2376.docx` | Full comparative analysis paper |
