Object Detection using YOLOv7 ONNX

This project implements object detection using the YOLOv7 model in the ONNX format. The script processes images and videos, detects objects, and visualizes the bounding boxes with class labels and confidence scores.

Features

Supports image and video input.

Uses ONNX runtime for inference.

Configurable confidence threshold.

Draws bounding boxes with class labels.

Installation

Prerequisites

Make sure you have Python installed (>=3.6).

Install dependencies

pip install -r requirements.txt

Usage

Run Object Detection

python detection.py --source <path_to_image_or_video> --names <path_to_class_names> --weights yolov7.onnx --tresh 0.25

Arguments:

--source: Path to image or video (use 0 for webcam).

--names: Path to the file containing class names.

--weights: Path to the ONNX weights file (default: yolov7.onnx).

--tresh: Confidence threshold (default: 0.25).

Example Usage:

python detection.py --source test.jpg --names data/class.names --weights yolov7.onnx --tresh 0.3

Model

The model used is YOLOv7 converted to ONNX format. Ensure that yolov7.onnx is in the project directory.

Output

The detected objects will be displayed with bounding boxes and class names in a pop-up window.
