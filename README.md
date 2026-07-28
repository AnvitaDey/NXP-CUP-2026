# NXP CUP INDIA 2026 – Computer Vision

YOLO11-based traffic sign detection module developed for the NXP Cup India 2026 autonomous vehicle competition.

The objective of this module is to perform real-time traffic sign detection from the onboard camera and provide detected sign information to the ROS navigation pipeline.

---

## Features

- YOLO11s object detector
- 9 traffic sign classes
- Real-time inference
- Optimized for autonomous RC vehicle deployment
- Pretrained using Ultralytics YOLO11

---

## Detected Classes

| ID | Class |
|----|-------|
| 0 | A |
| 1 | B |
| 2 | C |
| 3 | Left |
| 4 | Right |
| 5 | Straight |
| 6 | X |
| 7 | Y |
| 8 | Z |

---

## Model

Architecture:

YOLO11s

Input Resolution:

512 × 512

Training Images:

1896

Validation Images:

90

Framework:

Ultralytics YOLO11

---

## Performance

| Metric | Score |
|---------|------:|
| Precision | 97.7% |
| Recall | 96.0% |
| mAP@50 | 96.8% |
| mAP@50-95 | 73.7% |

Training performed on an NVIDIA Tesla T4 GPU using Kaggle.

---

## Repository Structure
