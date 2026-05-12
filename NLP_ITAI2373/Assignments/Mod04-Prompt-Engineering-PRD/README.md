# Mod04 — Prompt Engineering → Product Requirement Document (PRD)

## Problem Statement

Simulate the workflow of an AI-augmented product manager — using progressive prompt engineering techniques to transform a vague app idea into a structured, professional-grade Product Requirement Document (PRD).

## Approach

Four-task progressive prompting assignment using the Gemini API:

1. **Task 1 — Zero-Shot Baseline (The "Lazy PM"):** Asked the model simply: *"Write a PRD for FridgeChef."* Output was analyzed for vagueness — generic headers, unspecific requirements like "The app should be fast."

2. **Task 2 — Few-Shot Prompting:** Provided example PRD sections as context before the request. Observed how the model's output adopted the demonstrated structure and specificity level.

3. **Task 3 — Chain-of-Thought (Step-by-Step):** Instructed the model to reason through user problems, technical constraints, and success metrics before writing. Compared depth and precision against Tasks 1 and 2.

4. **Task 4 — Persona + Constraints:** Assigned the model a senior PM persona with explicit format constraints (required sections, word limits per section, measurable success criteria). Produced the most structured and deployable output.

## Results

Each prompting technique produced measurably better output than the previous. The zero-shot PRD was generic; the persona + constraints version included specific user stories, defined technical requirements, and quantifiable success metrics. The progression made the impact of prompt design concrete and visible.

## Key Findings

Prompt engineering is not hacking the model — it is communicating your requirements precisely. The same model produced dramatically different quality outputs based solely on how the task was framed. Persona assignment and explicit constraints were the highest-leverage techniques, turning a vague request into a professional deliverable without changing a single model parameter.

## Technologies Used

Python · Google Gemini API (`google-generativeai`) · Google Colab (Secrets for API key)

## How to Run

1. Set your `GOOGLE_API_KEY` in Colab Secrets (Runtime → Manage secrets)
2. Open `Mod04_FranciscoMedina_ITAI2373.ipynb` in [Google Colab](https://colab.research.google.com/)
3. Run all cells in order

## Files

| File | Description |
|---|---|
| `Mod04_FranciscoMedina_ITAI2373.ipynb` | Full prompt engineering assignment notebook |
