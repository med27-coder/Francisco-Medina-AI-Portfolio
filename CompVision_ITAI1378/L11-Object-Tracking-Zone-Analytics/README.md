# L11 — Real-Time Object Tracking & Zone-Based Analytics

## Problem Statement

Go beyond frame-by-frame object detection to persistent object tracking — following individual objects across video frames and using defined spatial zones to trigger analytics events based on where objects move.

## Approach

Extended the YOLO pipeline from Module 09 with a full tracking and zone analytics system:

1. **Object Tracking:** Integrated a tracking algorithm with YOLOv8 so each detected object receives a persistent ID across frames. The system follows individual entities (people, vehicles, etc.) even as they move through the scene.
2. **Zone Definition:** Drew spatial zones over the video frame (entry zones, exit zones, restricted areas) as geometric regions.
3. **Zone Analytics:** At each frame, determined which tracked objects were inside each zone. Triggered configurable events — counts, alerts, timestamps — when objects entered or exited zones.
4. **Output:** Annotated video frames with bounding boxes, object IDs, zone overlays, and real-time event readouts.

## Results

Built a working real-time tracking pipeline with zone-based event detection. The system could count object crossings, flag zone intrusions, and log dwell time — capabilities directly applicable to retail analytics, security monitoring, and traffic management.

## Key Findings

Object tracking and object detection are fundamentally different problems. Detection asks "what is in this frame?" — tracking asks "where did this specific entity go?" Adding persistent IDs unlocks a whole new category of analytics that frame-level detection cannot provide. Zone-based logic demonstrates how CV systems translate raw visual data into actionable business intelligence.

## Technologies Used

- Python, Ultralytics YOLOv8 (with built-in tracker), OpenCV (`opencv-python`), Requests
- Google Colab

## Dataset / Input

Video file or stream provided at runtime. YOLOv8 weights download automatically. No large dataset upload required.

## How to Run

Open `L11_Medina_Francisco_ITAI1378.ipynb` in [Google Colab](https://colab.research.google.com/) and run all cells in order. A sample video source is provided within the notebook.

## Files

| File | Description |
|---|---|
| `L11_Medina_Francisco_ITAI1378.ipynb` | Full tracking & zone analytics notebook |
