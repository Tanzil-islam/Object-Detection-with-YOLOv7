# 🌟 Object Detection using YOLOv7 ONNX

This project leverages the power of **YOLOv7 in ONNX format** to perform object detection on images and videos. The script efficiently detects objects, highlights them with bounding boxes, and labels them with confidence scores.

---

## 🚀 Features
✅ Supports both image and video input
✅ Uses **ONNX runtime** for fast inference
✅ Adjustable confidence threshold
✅ Visualizes detected objects with bounding boxes and labels

---

## 🔧 Installation
### 📌 Prerequisites
Ensure **Python (>=3.6)** is installed on your system.

### 📥 Install dependencies
```bash
pip install -r requirements.txt
```

---

## 🎯 Usage

### ▶ Run Object Detection
```bash
python detection.py --source <path_to_image_or_video> --names <path_to_class_names> --weights yolov7.onnx --tresh 0.25
```

### 🔹 Arguments:
- `--source` → Path to the image or video (use `0` for the webcam)
- `--names` → Path to the file containing object class names
- `--weights` → Path to the ONNX weights file *(default: `yolov7.onnx`)*
- `--tresh` → Confidence threshold *(default: `0.25`)*

### 📌 Example Usage:
```bash
python detection.py --source test.jpg --names data/class.names --weights yolov7.onnx --tresh 0.3
```

---

## 🧠 Model
The project utilizes **YOLOv7**, converted into the **ONNX format** for efficient inference. Ensure the `yolov7.onnx` file is present in the project directory.

---

## 📊 Output
Once executed, the script will display detected objects with bounding boxes and class labels in a **pop-up window**.

### 🖼 Example Detection Output
![Detection Example](path_to_your_image.jpg)

---

🔥 **Happy Coding & Object Detecting!** 🚀

