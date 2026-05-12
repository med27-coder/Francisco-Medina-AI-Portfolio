# L11 — Real-Time Object Tracking & Zone-Based Analytics

## What I Did

Extended frame-by-frame object detection into persistent object tracking — assigning stable IDs to individual objects across video frames. Added spatial zone definitions over the video frame and built event logic that fires when tracked objects enter or exit defined zones.

## What I Learned

Object tracking and object detection are different problems. Detection asks "what is in this frame?" — tracking asks "where did this specific entity go?" Persistent IDs unlock an entirely new category of analytics: dwell time, crossing counts, zone intrusions, and movement paths. These are exactly the capabilities used in retail analytics, traffic management, and security monitoring at scale.

## Challenges

Handling ID reassignment when objects temporarily leave the frame and reappear required understanding how YOLOv8's built-in tracker manages identity continuity. Defining zone boundaries as normalized coordinates (rather than pixel values) so they scale correctly across different video resolutions was also a non-obvious step.

## Technologies Used

Python · Ultralytics YOLOv8 (with tracker) · OpenCV · Requests · Google Colab

## How to Run

Open `L11_Medina_Francisco_ITAI1378.ipynb` in [Google Colab](https://colab.research.google.com/) and run all cells. A sample video source is provided in the notebook.

## Files

| File | Description |
|---|---|
| `L11_Medina_Francisco_ITAI1378.ipynb` | Full tracking and zone analytics notebook |
