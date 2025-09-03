# 🚦 Applied AI Lab – Project 3: Object Detection with YOLO

## 📌 Project Overview

This project is part of the Applied AI Lab series 
Project 3/6
The goal was to build an object detection model using YOLO to detect vehicles and traffic objects in images and videos.

Some Output (detected images):

https://github.com/Zahraa28/Object-Detection-with-YOLO/blob/main/output_task.mp4
https://github.com/Zahraa28/Object-Detection-with-YOLO/blob/main/b8ea6dd9130d82a3b6163bc3aaa823d3.jpg
https://github.com/Zahraa28/Object-Detection-with-YOLO/blob/main/ca746f20cdb24209cc407a88d42eb912.jpg
https://github.com/Zahraa28/Object-Detection-with-YOLO/blob/main/5abd8287f8cc969e0644f73cf40142d5.jpg
https://github.com/Zahraa28/Object-Detection-with-YOLO/blob/main/8eb6ae806d383a68998e792fa8941d34.jpg

Key steps included:

Organizing datasets (images + XML annotations).

Extracting frames from YouTube videos using pytubefix.

Visualizing bounding boxes.

Training YOLO with custom objects.

Using data augmentation to improve performance and generalization.



---

## 📂 Dataset

DhakaAI – [https://www.kaggle.com/datasets/rifat963/dhakaai-dhaka-based-traffic-detection-dataset]

Extracted frames from YouTube traffic videos (Dhaka, >5 minutes).

Dataset includes:

Pre-annotated images with XML files.
Additional custom categories: three-wheelers, garbage vans, SUVs.



---

## ⚙️ Methods & Workflow

### 1. Data Organization

Loaded images and paired them with annotations.

Separated data into training and validation sets.



### 2. Video Processing

Extracted frames from YouTube videos using pytubefix.

Converted video frames into dataset samples.



### 3. YOLO Training

Used YOLO model for object detection.

Learned three loss components:

Missing object

Wrong location

Wrong class




### 4. Data Augmentation

Applied transformations with TorchVision V2:

RandomHorizontalFlip

RandomRotation

ColorJitter


Skipped VerticalFlip (not realistic for cars on streets).

Post that I explain Data Augmentation:
👉 [https://www.linkedin.com/posts/al-zahraa-mohamed-608360247_dataaugmentation-deeplearning-machinelearning-activity-7363202717504229376-zusK?utm_source=share&utm_medium=member_desktop&rcm=ACoAAD0ZPWgBtmMM-jRkxTAI0AP7y9wAWa1ig2w]

### 5. Model Deployment

Applied trained YOLO model on images and videos of Istanbul traffic.

Successfully detected vehicles in real-world traffic scenes.





---

## 📊 Results

Improved generalization with augmentation.

Successfully detected traffic objects in Istanbul datasets.


### 🔎 Example Outputs



---

📚 Key Learnings

How to organize datasets with images + annotations.

Using YOLO for object detection tasks.

Understanding loss functions in YOLO.

The role of data augmentation in improving predictions.

Adding new objects into a YOLO model.

