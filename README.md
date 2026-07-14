# meal-ingredient-detection
Tier 1 computer vision project for detecting common meal ingredients using YOLO11.

# Meal Ingredient Detection: What's on My Plate?

## Project Information

**Student:** Alissa Canesim Bento

**Course:** ITAI 1378 – Computer Vision and AI

**Project Tier:** Tier 1

### Tier Justification

This project is designed as a Tier 1 application because it focuses on object detection using a pretrained YOLO11 model to detect common meal ingredients. If time allows, the project may later be expanded into recipe suggestions as a natural Tier 2 extension.

---

# Problem Statement

Preparing meals often involves multiple ingredients, but identifying them manually from a photo can be time-consuming and inconsistent. This project aims to develop a computer vision application that automatically detects common ingredients in meal images. The detected ingredients can serve as the foundation for future applications such as recipe recommendations and meal organization.

---

# Solution Overview

The application will receive a meal image as input and use a YOLO11 object detection model to detect common ingredients. The output will be an annotated image displaying the detected ingredients, their locations, and confidence scores.

---

# Technical Approach

**Computer Vision Technique**
- Object Detection

**Model**
- YOLO11

**Framework**
- Ultralytics + PyTorch

**Development Environment**
- Google Colab

YOLO11 was selected because it provides fast and accurate object detection while remaining efficient enough to run in Google Colab.

---

# Data Plan

**Source**
- Public ingredient detection dataset (Roboflow Universe or Kaggle)

**Dataset Size**
- A subset of a publicly available dataset

**Labels**
- Selected common meal ingredients (e.g., tomato, lettuce, chicken, cheese, onion)

The selected dataset will be divided into training, validation, and testing sets following the YOLO11 format.

---

# Success Metrics

**Primary Metric**
- mAP50 ≥ 0.70

**Secondary Metric**
- Inference time < 1 second per image

---

# Milestone Plan

| Phase | Goal | Milestone |
|-------|------|-----------|
| 🧭 Blueprint | Define the project scope, dataset, and technical approach | Midterm submitted |
| 🔌 First Working Demo | Run a pretrained YOLO11 model on sample meal images | End-to-end pipeline working |
| 🛠 Make It Yours | Train the model with the selected ingredient dataset and test ingredient detection | System works on the selected problem |
| 📈 Improve and Measure | Evaluate performance using mAP50 and inference time | Metrics recorded |
| 🎥 Package and Present | Final README, slides, demo video, and project documentation | Final project submitted |

---

# Top Risks and Plan B

## Risk 1
A suitable public ingredient detection dataset may not be available.

**Plan B**
Use another publicly available dataset from Roboflow Universe or Kaggle with similar ingredient annotations.

## Risk 2
The model may not achieve the desired detection performance.

**Plan B**
Reduce the number of ingredient classes and fine-tune the model using a smaller subset of well-annotated images.

---

# AI Usage

The AI usage log for this project is available in:

`docs/AI_usage_log.md`
