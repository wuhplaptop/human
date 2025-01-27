# Human-50e-11n

## Model Overview

**Architecture:** YOLOv11  
**Training Epochs:** 50  
**Batch Size:** 32  
**Optimizer:** auto  
**Learning Rate:** 0.0005  
**Data Augmentation Level:** Moderate

## Training Metrics

- **mAP@0.5:** 0.91583

## Class IDs

| Class ID | Class Name |
|----------|------------|
| 0 | Person |


## Datasets Used

- detect-human-lg2ng_v1
- human-detection-grmvx_v1
- human-detection-p8c2v_v1
- human-pysi7_v3
- humans-ziarm_v2
- people-4evn7-fqlf8-d887c_v3
- people-4evn7_v2
- person-dataset-kzsop-vemv4-h1uoh-q5vtx_v2
- tello-olz2y_v5

## Class Image Counts

| Class Name | Image Count |
|------------|-------------|
| Person | 10865 |


## Description

This model was trained using the YOLOv11 architecture on a custom dataset. The training process involved 50 epochs with a batch size of 32. The optimizer used was **auto** with an initial learning rate of 0.0005. Data augmentation was set to the **Moderate** level to enhance model robustness.

## Usage

To use this model for inference, follow the instructions below:

```python
from ultralytics import YOLO

# Load the trained model
model = YOLO('best.pt')

# Perform inference on an image
results = model('path_to_image.jpg')

# Display results
results.show()
