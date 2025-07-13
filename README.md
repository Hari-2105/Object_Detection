# Object_Detection
# 🧠 YOLOv8 IP Camera Object Detection System

This project is a **Flask-based real-time object detection system** using **YOLOv8** and **IP camera streams**. It leverages computer vision to detect objects and allows users to control camera features like rotation, flashlight, and camera switch from a web interface.

---

## 📌 Features

- 📹 Real-time object detection via IP Camera stream
- 🧠 YOLOv8 and YOLOv8-seg (segmentation) supported
- 🔀 Supports multiple camera views
- 🕹️ Camera control: rotate, switch, flashlight
- 🧪 Additional CLI testing scripts included for model verification

---

## 🗂️ Project Structure

Object_Detection/
│
├── webhosting.py # 🔥 Flask entry point
├── vediofetching.py # Basic IP cam reader
├── templates/
│ └── index.html # 🌐 Web UI
├── utils/
│ └── coco.txt # 🏷️ Class names (COCO 80)
├── weights/
│ ├── yolov8n.pt # YOLOv8 detection model

├── temp/
│ ├── yolo.py # CLI-based YOLOv8 segmentation + tracking
│ ├── yolov1.py # YOLOv8 webcam detection
│ ├── objectdetection.py # YOLOv5 OpenCV DNN fallback
└── requirements.txt # 📦 Python dependencies

yaml
Copy
Edit

---

## 🚀 Getting Started

### 🔧 Installation

```
git clone https://github.com/Hari-2105/Object_Detection.git
cd Object_Detection
pip install -r requirements.txt
```

### 📦 Requirements
Make sure the following are installed:

Python 3.8+

OpenCV

Flask

ultralytics

numpy

requests

# 💻 Running the App
```
python webhost.py
```
Then open http://127.0.0.1:5000 in your browser.

### 🧪 Sample CLI Detections
```
# YOLOv8 object detection via webcam
python temp/yolov1.py

# YOLOv8 segmentation and tracking
python temp/yolo.py

# YOLOv5 DNN fallback detector
python temp/objectdetection.py
```
# 📸 Screenshots
| Web Interface and Detection Output |
|------------------------------------|
| ![Object_detection_output](Object_Detection/Outputs/Screenshot%20(78).png) |


# 🎯 Future Enhancements
- 📲 Mobile-friendly UI

- 🧪 Custom object class training support

- 🧠 Real-time event logging and analytics

- 🌐 Cloud deployment (AWS/GCP/Azure)

# 🙋 Author
👨‍💻 Developed by Harish V
