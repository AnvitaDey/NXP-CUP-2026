# NXP CUP India 2026 – Computer Vision

This repository contains the Computer Vision module developed for the **NXP CUP India 2026** autonomous RC car competition.

The objective of this module is to perform real-time traffic sign detection using **YOLO11s**, enabling the vehicle to identify road signs and provide detection results to the navigation and control pipeline.

---

## Model

- **Architecture:** YOLO11s
- **Framework:** Ultralytics YOLO
- **Input Size:** 512 × 512
- **Number of Classes:** 9

### Detected Classes

- A
- B
- C
- Left
- Right
- Straight
- X
- Y
- Z

---

## Model Performance

| Metric | Score |
|--------|-------:|
| Precision | **97.7%** |
| Recall | **96.0%** |
| mAP@50 | **96.8%** |
| mAP@50-95 | **73.7%** |

Training was performed on an NVIDIA Tesla T4 GPU using transfer learning with the pretrained YOLO11s model.

---

## Repository Structure

```
NXP-CUP-2026/
│
├── models/
│     └── best.pt          # Trained YOLO11s model
│
├── metrics/
│     ├── results.png
│     ├── confusion_matrix.png
│
├── dataset/
│     └── data.yaml        # Dataset configuration
│
└── README.md
```

---

## Notes

- `models/best.pt` contains the final trained model.
- `metrics/` contains evaluation plots and training results.
- The dataset is **not included** in this repository. Only the dataset configuration (`data.yaml`) is provided.

---

## Authors

Developed for **NXP CUP India 2026**  
Team 4249
