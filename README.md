# 🔍 Industry-Oriented Object Detection using YOLOv8

![Python](https://img.shields.io/badge/Python-3.10-blue)
![YOLOv8](https://img.shields.io/badge/Model-YOLOv8-orange)
![Framework](https://img.shields.io/badge/Framework-PyTorch-red)
![Dataset](https://img.shields.io/badge/Dataset-COCO-green)
![Platform](https://img.shields.io/badge/Platform-Google%20Colab-yellow)

## 📌 Project Overview
This project is developed as part of the **RISE Internship Program**
under the **Deep Learning & Neural Networks** track. It implements
an industry-grade object detection system capable of identifying
and localizing multiple objects in real-world images and video frames
using the state-of-the-art **YOLOv8** architecture.

---

## 🎯 Objective
To build a deep learning object detection pipeline that:
- Detects and classifies multiple objects in images
- Draws bounding boxes with confidence scores
- Evaluates model performance using standard metrics
- Works on real-world images and video frames

---

## 🧠 Model Architecture
| Component     | Detail                        |
|---------------|-------------------------------|
| Model         | YOLOv8n (Nano)                |
| Framework     | PyTorch + Ultralytics         |
| Backbone      | CSPDarknet                    |
| Neck          | PANet (Feature Pyramid)       |
| Head          | Decoupled Detection Head      |
| Dataset       | COCO (80 classes)             |
| Input Size    | 640 × 640                     |
| Confidence    | ≥ 0.40                        |
| NMS IoU       | 0.45                          |

---

## 🛠️ Tech Stack
- **Language:** Python 3.10
- **Deep Learning:** PyTorch, Ultralytics YOLOv8
- **Computer Vision:** OpenCV
- **Visualization:** Matplotlib
- **Platform:** Google Colab (GPU — T4)
- **Tools:** NumPy, Pillow, Requests

---

## 📂 Project Structure
```
object-detection-yolov8/
│
├── object_detection.ipynb   # Main Colab notebook
├── results/                 # Output detection images
├── requirements.txt         # Dependencies
└── README.md                # Project documentation
```

---

## 🚀 How to Run

### 1. Open in Google Colab
Click the badge below to open directly:

[![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1D4z2k1i8G51XD1tFLP2nw_kGKmtQeiEr?usp=sharing)

### 2. Install dependencies
```python
!pip install ultralytics opencv-python-headless matplotlib numpy
```

### 3. Run detection
```python
from ultralytics import YOLO
model = YOLO('yolov8n.pt')
results = model.predict('your_image.jpg', conf=0.4)
```

---

## 📊 Evaluation Metrics
| Metric           | Score  |
|------------------|--------|
| mAP @ 0.50       | 0.63+  |
| mAP @ 0.50:0.95  | 0.45+  |
| Precision        | 0.72+  |
| Recall           | 0.58+  |

---

## 🏷️ Detected Object Classes (Sample)
Person · Car · Bus · Truck · Bicycle · Dog · Cat ·
Chair · Sofa · TV · Bottle · Cup · Phone · and 67 more...

---

## 🎓 Internship Details
| Field        | Detail                            |
|--------------|-----------------------------------|
| Program      | RISE Internship                   |
| Track        | Deep Learning & Neural Networks   |
| Project      | Industry-Oriented Object Detection|
| Tools Used   | Python, PyTorch, YOLOv8, Colab    |

---

⭐ If you found this project helpful, please give it a star!

---
