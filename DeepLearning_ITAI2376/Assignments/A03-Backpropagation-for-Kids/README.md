# A03 — Backpropagation for Kids

**Team 2:** Francisco Medina · Richard Rodriguez · Rida Kashan · Yoana Cook  
**Date:** 02.04.2026

## Problem

Explain backpropagation — one of deep learning's most mathematically dense concepts — to a non-technical audience (younger students / general public) without losing accuracy.

## Approach

6-section presentation built around two core analogies: learning to ride a bike (iterative improvement through mistakes) and baking a salty cake (proportional blame assignment across layers). Deliberately avoided equations; used visual diagrams, comics-style imagery, and a step-by-step forward/backward pass walkthrough.

## Key Concepts Covered

- Forward pass → loss measurement → backward pass → weight adjustment → repeat
- Why backpropagation is more powerful than random trial-and-error: it pinpoints *exactly* which connections caused the error and *by how much*
- Small, stable weight updates (e.g., 0.50 → 0.52 → 0.55 → 0.60) vs. large destructive jumps
- Real-world framing: the same loop that trains a chihuahua/muffin classifier runs inside every modern AI

## Key Findings

The baking analogy was the most effective teaching tool — "sending the blame backward through layers" maps directly to the chain rule without naming it. Audiences at any level can grasp proportional responsibility.

## Files

| File | Description |
|---|---|
| `A03_team02_franciscomedina_ITAI2376.pdf` | Full 11-slide presentation deck |
