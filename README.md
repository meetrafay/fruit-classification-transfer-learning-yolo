# 🍎 Fruit Classification with Transfer Learning & YOLOv8

A computer vision project for classifying fruit images using Transfer Learning with pretrained CNN models (ResNet50, VGG16, EfficientNet-B0) and YOLOv8 (used as a classifier). Includes OpenCV-based preprocessing, augmentation, and visualization tasks.

---

## 📁 Dataset

**Source:** [Kaggle Fruits 360 Dataset (Small Subset)](https://www.kaggle.com/datasets/moltean/fruits)

The dataset is organized into subfolders per fruit class:

dataset/
├── train/
│ ├── Apple/
│ ├── Banana/
│ └── ...
└── val/
├── Apple/
├── Banana/
└── ...


---

---

## 🧠 Models Used

### 🔹 Transfer Learning (Image Classification)
- ✅ ResNet50
- ✅ VGG16
- ✅ EfficientNet-B0

**Steps:**
- Used pretrained weights from ImageNet
- Replaced final classification layer with 15 output classes
- Used data augmentation (flip, rotate, zoom)
- Evaluated using accuracy, precision, recall, F1-score, confusion matrix

### 🔹 YOLOv8 (Used as Image Classifier)
- Model: `yolov8n-cls.pt` from Ultralytics
- Trained on same folder-based dataset format
- Used `Ultralytics` Python library to train and validate
- Compared YOLO classifier accuracy with CNN models

---

## 🧪 OpenCV Preprocessing Tasks

Included visualizations for:
- ✅ Loading sample images
- ✅ Grayscale conversion
- ✅ Gaussian Blur
- ✅ Canny edge detection
- ✅ Resize and padding
- ✅ Custom augmentations (horizontal flip, brightness, rotation)

---

## 📊 Evaluation & Results

| Model          | Accuracy | Precision | Recall | F1-Score | Training Time |
|----------------|----------|-----------|--------|----------|----------------|
| ResNet50       | ✅        | ✅         | ✅      | ✅        | Moderate       |
| VGG16          | ✅        | ✅         | ✅      | ✅        | Slow           |
| EfficientNet-B0| ✅        | ✅         | ✅      | ✅        | Fast           |
| YOLOv8n-cls    | ✅        | ✅         | ✅      | ✅        | Very Fast      |

📌 Final report includes training curves, confusion matrices, and model comparison insights.

---


