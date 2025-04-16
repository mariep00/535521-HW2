# NYCU Selected Topics in Visual Recognition using Deep Learning 2025 Spring - HW2

**Student ID**: 313551818  
**Name**: Marie Picquet

---

## Introduction

This repository contains the implementation for Homework 2: Digit Recognition using Faster R-CNN. The objective is to detect individual digits in images and reconstruct full digit sequences. The model is based on Faster R-CNN with a MobileNetV3 Large backbone and FPN, implemented using PyTorch's `torchvision` detection module.

The project is divided into two tasks:
- **Task 1**: Detect each digit using bounding boxes and classify them (0–9).
- **Task 2**: Predict the full number in the image using the output from Task 1.

---

## How to Install

1. Clone the repository or open the notebook in Google Colab.  
2. The code was tested using the following environment:
   - Python 3.10+
   - PyTorch (>=2.0)
   - torchvision
   - numpy
   - matplotlib
   - tqdm
   - PIL

If running locally, install dependencies with:

```bash
pip install -r requirements.txt
```


3. Extract Dataset
Update the dataset extraction path to your own Google Drive or local directory and change the necessary paths

```python
# Dataset path
data_root = "/content/drive/MyDrive/NYCU/HW2/nycu-hw2-data"
```
Moreover update the paths in inference and predictions aswell as where to save the predictions.

4. Directory structure
   
  nycu-hw2-data/
├── train/
├── valid/
├── test/
├── train.json
└── valid.json


5. Performance Snapshot

Competition test score Task 1: 38%
Competition test score Task 2: 81%
<img width="1157" alt="Screenshot 2025-04-16 at 21 00 12" src="https://github.com/user-attachments/assets/91476182-3ddd-4f6f-939c-91a03cba0c0c" />


