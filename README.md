![vertopal com_capture_20241112115242786](https://github.com/user-attachments/assets/f48d821a-2387-4ccc-a6da-b733e6c6aa05)

# Real-Time Object Detection with YOLOv3

This project implements a real-time object detection system using the YOLOv3 (You Only Look Once) model with OpenCV and Python. The system detects and labels objects from a live video feed, displaying them with bounding boxes and confidence scores.

## Project Overview

The objective of this project is to create a real-time object detection application that can accurately identify and label objects from the COCO dataset in a webcam video feed. The project leverages the YOLOv3 model's pre-trained weights for efficient and accurate detection.

## Requirements

- **Python 3.x**
- **OpenCV** (`opencv-python`)
- **NumPy** (`numpy`)

### Installation

To install the required libraries, run:

```bash
pip install opencv-python numpy
```

## YOLO Files
- yolov3.cfg: YOLO model configuration file.
- yolov3.weights: YOLO model weights file.
- coco.names: COCO labels file containing object names.

# Code Overview
## Functions
- load_labels(labels_path): Loads the class labels (object names) from the coco.names file.
- load_yolo_model(config_path, weights_path): Loads the YOLO model with specified configuration and weights, and retrieves the output layer names.
- perform_detection(net, image, output_layers): Processes a single frame for object detection, returning bounding boxes, confidence scores, and class IDs for each detected object.
- draw_predictions(image, boxes, confidences, class_ids, labels): Draws bounding boxes, labels, and confidence scores on detected objects in the video feed.


When you run the script, a live video feed will open, displaying detected objects with bounding boxes, labels, and confidence scores. Press "q" to exit the application.

