# Blister Detection Project

## Overview
A YOLOv8-based blister detection system implementing a multi-stage approach combining synthetic and real data training. The system features an interactive interface for testing different models and analyzing blister characteristics.

## Performance Results
Best Model Performance (Synthetic Training):
- Precision: 97.5%
- Recall: 85.3%
- mAP50: 90.5%
- mAP50-95: 78.1%

## Available Models

### Base Models
- YOLOv8n (Nano version)
- YOLOv8s (Small version)
- YOLOv11n

### Trained Models
1. Synthetic Training Model
  - Best for synthetic-like images
  - Location: `runs/detect/yolov8s_synthetic/weights/best.pt`

2. Fine-tuned Model
  - Optimized for real-world images
  - Location: `runs/detect/yolov8s_real_finetuned/weights/best.pt`

3. Combined Dataset Model
  - Best overall performance
  - Location: `yolo_results/yolov8s_combined/weights/best.pt`

## Features

### Detection Capabilities
- Multiple blister detection
- Confidence scoring
- Size analysis
- Quality grading

### Interactive Interface
- Multiple image upload
- Batch processing
- Real-time analysis
- Detailed results visualization

### Analysis Output
- Blister count and location
- Confidence levels
- Size distribution
- Quality grade assessment

## Setup Instructions
1. Install required packages using requirements.txt
2. Open notebook in Google Colab
3. Mount Google Drive
4. Load desired model
5. Use interactive interface for testing

## Model Selection Guide
- For Fast Testing: Use YOLOv8n
- For Real-World Applications: Use Fine-tuned Model
- For Best Overall Results: Use Combined Dataset Model

## Note
The complete implementation, including training procedures and interactive testing interface, is available in the notebook `blister_detection_ml.ipynb`.
