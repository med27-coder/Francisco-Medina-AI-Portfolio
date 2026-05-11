# L10 — Building an Agent with a Framework

## Problem Statement

Move beyond building agents from scratch by implementing a structured agent using a pre-built framework — understanding how production-grade agent systems organize tools, memory, and workflow into reusable, scalable components.

## Approach

Built a structured agent using pure Python to understand framework internals before adopting a library. The lab modeled the three core pillars of any agent framework:

1. **Tools:** Pre-defined callable functions the agent can invoke (e.g., weather lookup, data retrieval).
2. **Memory:** State tracking across interactions so the agent can build on previous context.
3. **Workflow:** Orchestration logic that decides which tool to call, when to call it, and what to do with results.

A sample weather-answering agent demonstrated the complete framework in action.

## Results

Successfully implemented a mini agent framework from scratch, then understood how production frameworks (LangChain, AutoGen, etc.) abstract these same components. The exercise clarified what "using an agent framework" actually means under the hood.

## Key Findings

Agent frameworks are not magic — they are well-structured implementations of the same core loop: observe input → select tool → execute → update memory → respond. Building one from scratch makes debugging real framework-based agents significantly easier, because you understand exactly what each layer is responsible for.

## Technologies Used

- Python (standard library only — no external dependencies)
- Google Colab / Jupyter

## How to Run

Open `L10_Medina_Francisco_ITAI1378.ipynb` in [Google Colab](https://colab.research.google.com/) or any Jupyter environment and run all cells in order. No installations required.

## Files

| File | Description |
|---|---|
| `L10_Medina_Francisco_ITAI1378.ipynb` | Full agent framework lab notebook |
