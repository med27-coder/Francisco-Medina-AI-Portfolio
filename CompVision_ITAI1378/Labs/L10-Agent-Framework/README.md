# L10 — Building an Agent Framework

## What I Did

Built a structured agent framework from scratch in pure Python — implementing the three core pillars of any production agent system: tools (callable functions), memory (state across interactions), and workflow (orchestration logic). Used a sample weather-answering agent to demonstrate the complete framework.

## What I Learned

Agent frameworks are not magic — they are clean implementations of the same core loop: observe input → select tool → execute → update memory → respond. Building one from scratch makes debugging real framework-based agents significantly easier, because you understand what each layer is responsible for. Every LangChain or AutoGen abstraction maps directly to one of these three components.

## Challenges

Designing the tool selection logic — how the agent decides which tool to call given a user query — required thinking carefully about intent classification before any AI techniques were available to automate it. The memory component also raised the question of what to remember vs. discard across turns.

## Technologies Used

Python (standard library only) · Google Colab

## How to Run

Open `L10_Medina_Francisco_ITAI1378.ipynb` in [Google Colab](https://colab.research.google.com/) and run all cells. No installations required.

## Files

| File | Description |
|---|---|
| `L10_Medina_Francisco_ITAI1378.ipynb` | Full agent framework notebook |
