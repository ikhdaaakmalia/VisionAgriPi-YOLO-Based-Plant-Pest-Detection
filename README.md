# VisionAgri-Pi  
Automated Plant Pest Detection System using Computer Vision

## Overview
VisionAgri-Pi is an end-to-end computer vision system designed to automatically detect and classify plant pests using object detection models. The system is built to support early pest monitoring in agriculture and is deployed on a Raspberry Pi for real-world usage.

## Problem Statement
Manual pest identification is time-consuming and highly dependent on human expertise, which can lead to delayed intervention and crop damage. This project aims to automate pest detection to improve monitoring efficiency and decision-making in agricultural environments.

## Dataset
- Approximately 5,000 annotated images  
- 8 plant pest classes  
- Source: Roboflow  
- Data split:
  - Training: 70%
  - Validation: 20%
  - Testing: 10%

## Methodology
- Dataset preparation and annotation management  
- Data preprocessing and augmentation  
- Object detection model training using **YOLOv5** and **YOLOv8**  
- Training conducted on **Google Colab** with 100–300 epochs  
- Ablation study to analyze the impact of model configurations on performance  

## Evaluation Metrics
- mAP@0.5  
- mAP@0.5–0.95  
- Precision  
- Recall  

## Results
Based on evaluation results, YOLOv8 demonstrated more stable and consistent performance compared to YOLOv5 across the defined metrics. The ablation study highlighted the influence of data augmentation strategies and training configurations on detection accuracy.

## Deployment
The trained model was integrated into a **Raspberry Pi–based monitoring system**, featuring:
- Real-time pest detection on edge devices  
- Web-based dashboard for monitoring results  
- Telegram notification system for detection alerts  

## Limitations
- Model performance is affected by image quality and lighting conditions  
- Limited dataset diversity for certain pest classes  

## Future Improvements
- Expanding dataset size and class diversity  
- Optimizing inference speed for edge deployment  
- Enhancing robustness under varying environmental conditions  

## Tools & Technologies
- Python  
- YOLOv5, YOLOv8  
- Roboflow  
- Google Colab  
- Raspberry Pi  

## Author
Ikhda Akmalia Putri
