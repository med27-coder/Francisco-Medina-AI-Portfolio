# L09 — AI Agent with Computer Vision

## What I Did

Built a working AI agent that uses YOLOv8 as its perception layer, implementing the Perception-Reasoning-Action (PRA) loop to create a system that monitors a video stream, detects events, and responds autonomously based on configurable rules.

## What I Learned

AI agents are more than accurate models — the reasoning layer is where intelligence lives. A perfectly accurate detector with poor reasoning logic still produces bad agent behavior. The PRA framework provides a clean mental model for any perception-based system: detect (perceive), evaluate rules (reason), trigger response (act). This pattern scales from a simple alarm system to complex autonomous vehicles.

## Challenges

Configuring the reasoning rules to be specific enough to be useful but general enough not to fire constantly required iteration. Handling edge cases — what happens when YOLO detects the same object across multiple frames — required thinking about state, not just individual detections.

## Technologies Used

Python · Ultralytics YOLOv8 · OpenCV · Requests · Google Colab

## How to Run

Open `Module_09_Lab_AI_Agents_FranciscoMedina_ITAI1378.ipynb` in [Google Colab](https://colab.research.google.com/) and run all cells. A sample video URL is included in the notebook.

## Files

| File | Description |
|---|---|
| `Module_09_Lab_AI_Agents_FranciscoMedina_ITAI1378.ipynb` | Full AI agent lab notebook |
