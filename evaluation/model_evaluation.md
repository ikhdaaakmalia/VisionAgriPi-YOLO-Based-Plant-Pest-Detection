# Model Evaluation

## Overview
The model evaluation was conducted using an ablation study approach to analyze the impact of each component on overall detection performance. This approach helps determine whether data augmentation and loss function adjustments significantly improve detection accuracy.

## YOLOv5 Evaluation

| Configuration              | Precision | Recall | mAP@50 | mAP@50–90 | F1-Score |
|---------------------------|-----------|--------|--------|-----------|----------|
| Baseline                  | 0.9268    | 0.9117 | 0.6248 | 0.6564    | 0.9192   |
| Data Augmentation         | 0.9244    | 0.9126 | 0.5865 | 0.6046    | 0.9184   |
| Loss Adjustment           | 0.9281    | 0.9125 | 0.6267 | 0.6541    | 0.9202   |
| Full Configuration        | 0.9222    | 0.9135 | 0.5754 | 0.6011    | 0.9178   |

## YOLOv8 Evaluation

| Configuration              | Precision | Recall | mAP@50 | mAP@50–90 | F1-Score |
|---------------------------|-----------|--------|--------|-----------|----------|
| Baseline                  | 0.9207    | 0.9092 | 0.6549 | 0.6669    | 0.9150   |
| Data Augmentation         | 0.9296    | 0.9156 | 0.6416 | 0.6292    | 0.9226   |
| Loss Adjustment           | 0.9255    | 0.9231 | 0.6748 | 0.6682    | 0.9243   |
| Full Configuration        | 0.9266    | 0.9224 | 0.6429 | 0.6279    | 0.9245   |

## Discussion
YOLOv5 demonstrated consistently high precision and recall across all configurations, indicating reliable object-background separation. However, performance gains from augmentation and loss adjustments were marginal, particularly in detecting small objects.

In contrast, YOLOv8 showed better adaptability to optimization techniques, achieving more stable performance across multiple metrics. Despite these improvements, detecting small pests under complex field conditions remains a challenge.
