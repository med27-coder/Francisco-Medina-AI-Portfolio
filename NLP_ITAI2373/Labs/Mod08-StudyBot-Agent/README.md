# Mod08 — StudyBot: Intelligent Agent with Tools, Reasoning & Memory

## What I Did

Built StudyBot — a fully functional AI agent using LangChain and LangGraph that goes far beyond a plain chatbot. StudyBot has real tools, a reasoning loop, and persistent memory across a conversation. Runs entirely locally via Ollama (Llama 3.2) with no API key required.

## What I Learned

The gap between a chatbot and an agent is tools plus a reasoning loop. A chatbot generates a response. An agent decides whether to call a tool, calls it, reads the result, and then responds — all in a structured graph. LangGraph's `StateGraph` makes this explicit: nodes are actions (LLM call, tool call), edges are decisions (should I use a tool or respond directly?). Memory is just state that persists across turns — once you see it as state management, it becomes straightforward.

## Challenges

Getting Ollama configured correctly as a local LLM backend was the main setup hurdle — the LLM had to be running at `http://localhost:11434` before the notebook could connect. Understanding LangGraph's message-passing model (why `add_messages` works the way it does) required reading the docs carefully before the flow clicked.

## Technologies Used

Python · LangChain · LangGraph · Ollama (Llama 3.2) · `langchain-ollama` · Google Colab / local environment

## How to Run

1. Install [Ollama](https://ollama.com) and run `ollama pull llama3.2` in terminal
2. Open `Mod08_StudyBot_FranciscoMedina_ITAI2373.ipynb` in Jupyter or Colab
3. Run all cells — Ollama serves as the LLM backend locally, no API key needed

## Files

| File | Description |
|---|---|
| `Mod08_StudyBot_FranciscoMedina_ITAI2373.ipynb` | Full StudyBot agent notebook |
