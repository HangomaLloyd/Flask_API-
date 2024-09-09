# Pothole Detection Using YOLOv8

This repository contains a custom object detection classifier to detect potholes on roads, using YOLOv8. It is a transition from the TensorFlow Object Detection API, previously used for this task, to the YOLOv8 model for more efficient and real-time detection.

## Overview

The model is designed to detect and differentiate between 4 different classes:

1. **Pothole** – Single pothole.
2. **Pothole Group** – More than two potholes or a large pothole.
3. **Car** – Cars on the road.


The focus of the model is to prioritize the detection of potholes and pothole 

## Implementation Steps

### 1. Gather Images and Labeling
- The dataset for pothole images was obtained from Kaggle.
- Image annotation was done using **LabelImg**, an open-source tool.
- For YOLOv8, labels must be converted to YOLO format (TXT files), containing bounding box coordinates for each class.

### 2. Environment Setup for YOLOv8
1. Install YOLOv8 by running:
   ```bash
   pip install ultralytics
   dataset/
├── images/
│   ├── train/
│   └── val/
└── labels/
    ├── train/
    └── val/

