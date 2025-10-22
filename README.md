# CCTV Pedestrian Tracking and Top-Down Projection

This project uses Ultralytics YOLO for pedestrian detection and tracking, combined with OpenCV to project each tracked path — originally recorded from an **eye-level camera view** — onto a **top-down (bird’s-eye) perspective** of the same video.  

The code demonstrates how to integrate object detection, trajectory tracking, and perspective transformation for visualizing crowd movement patterns.

---

- **Pedestrian Detection** – Uses YOLO (You Only Look Once) for accurate person detection in each frame.  
- **Object Tracking** – Maintains consistent IDs for each pedestrian across frames using YOLO’s built-in tracking or custom SORT/DeepSORT options.  
- **Top-Down Projection** – Applies homography transformation to map pedestrian positions from the perspective camera view to a top-down (planar) view of the same scene.  
- **Trajectory Visualization** – Draws each tracked pedestrian’s path over time on the top-down map.  
- **Video Output** – Exports both the annotated detection video and the projected top-down trajectory visualization.

---

 Requirements:
```bash
pip install ultralytics opencv-python numpy matplotlib
