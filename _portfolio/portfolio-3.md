---
title: "Custom Object Detection with YOLOv7: Dataset Curation, Training, and Real-Time Deployment"
excerpt: "Short description of portfolio item number 3<br/><img src='/images/saurabh/yolo/main.png'>"
collection: portfolio
---

This project involves training a YOLOv7 (You Only Look Once version 7) model to detect custom objects. The process included curating a custom image dataset, performing data annotation, and fine-tuning the YOLOv7 model to achieve optimal detection accuracy.

Key Features

-Custom Dataset Curation: Collected and annotated a dataset tailored for the target objects using tools like LabelImg.

-YOLOv7 Model Training: Fine-tuned YOLOv7 on the curated dataset using PyTorch and GPU acceleration for efficient training.

-Augmentation & Preprocessing: Applied image augmentation techniques (flipping, rotation, color jittering) to improve model generalization.

-Model Optimization: Tuned hyperparameters like learning rate, batch size, and anchor boxes to enhance performance.

-Real-Time Inference: Deployed the trained model for real-time object detection using OpenCV and a custom pipeline.

Tools & Technologies Used: \ 
YOLOv7, PyTorch, CUDA, OpenCV
LabelImg for annotation
Google Colab / Local GPU for training


<figure>
  <img src="/images/saurabh/yolo/1.jpg" alt="samples" width="600">
  <figcaption style="text-align: center;">Figure 1: Sample Testing 1</figcaption>
</figure>

<figure>
    <img src="/images/saurabh/yolo/2.jpg" alt="architecture" width="600">
    <figcaption style="text-align: center;">Figure 2: Sample Testing 2</figcaption>
  </figure>

  <figure>
    <img src="/images/saurabh/yolo/results.png" alt="architecture" width="600">
    <figcaption style="text-align: center;">Figure 3: Results</figcaption>
  </figure>

  <figure>
    <img src="/images/saurabh/yolo/F1_curve.png" alt="architecture" width="600">
    <figcaption style="text-align: center;">Figure 4: F1 Curve</figcaption>
  </figure>