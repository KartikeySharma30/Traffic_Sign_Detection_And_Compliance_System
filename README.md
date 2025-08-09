# **Traffic Sign Detection and Compliance System**

## Project Overview :
- This project implements a real-time traffic sign detection system using YOLOv8m for Autonomous and Semi-Autonomous driving assistance. The system identifies and classifies traffic signs from video feeds, provides voice alerts for compliance, and outputs annotated video results.

- By improving the detection accuracy (mAP@50: from 95.6% to 97.5%), this solution aims to ensure a safer and more reliable on-road ecosystem.

## Objective :

- Detect and classify traffic signs in real time using YOLOv8m.
- Provide auditory alerts to enhance driver awareness and compliance.
- Enable high-confidence detection through optimized thresholds.
- Demonstrate results with annotated video outputs.

## Dataset
- Source : GTSRB and pkdarabi-cardetection
- Structure:

  Train: 3,530 images

  Validation: 801 images

  Test: 638 images

- Format: YOLO-compatible with data.yaml mapping labels and bounding boxes.

Libraries: YOLOv8, OpenCV, PIL, Pandas, Matplotlib, MoviePy, Roboflow API

## Workflow
- Data Acquisition & Preparation
  > Download dataset via Kaggle API
  
  > Roboflow-provided annotations for training/validation/testing
  
  > Data mapped via data.yaml for YOLOv8 format

- Model Training
  > Trained YOLOv8m on the dataset
  
  > Fine-tuned confidence thresholds to improve detection accuracy
  
  > Achieved mAP@50: 97.5%

- Model Evaluation
  > Evaluated on test images and videos
  
  > Compared precision, recall, and mAP scores
  
  > Compliance System (Voice Alerts)

- Mapped each detected traffic sign to a predefined audio alert
  > Selected prediction from the last frame in which the sign appeared for highest confidence
  
  > Visualization & Output
  
  > Annotated video output with detected traffic signs and labels
  
  > Real-time video inference integrated with OpenCV and MoviePy

## Results 
- mAP@50 Improvement: 95.6% → 97.5%
- Real-time Capability: Achieved smooth frame-by-frame detection on video feed.
- Compliance Feature: Successfully mapped detections to voice alerts for enhanced driver assistance.


## Sample Output
