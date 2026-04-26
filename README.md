# Vehicle Safety Helmet Detection using YOLOv8

This repository contains a Jupyter Notebook for training a YOLOv8 model to detect safety helmets (hard hats) in various environments. It includes a complete pipeline for dataset preparation, model training, and inference.

## ✨ Features
- **YOLOv8 Core**: Leverages the power of Ultralytics YOLOv8 for high-accuracy object detection.
- **Dataset Support**: Compatible with both local datasets and Roboflow Universe datasets.
- **End-to-End Pipeline**: Includes environment setup, training, validation, and real-world prediction.
- **Visual Results**: Built-in visualization tools to inspect model performance on test images.

## 📁 Project Structure
- `helmet_detection.ipynb`: The main notebook for training and detection.
- `dataset_helmet/`: Local dataset directory.
  - `images/`: Dataset images.
  - `annotations/`: Corresponding YOLO format labels.

## 🚀 Getting Started

### Prerequisites
Ensure you have Python installed. You will need the following libraries:
```bash
pip install ultralytics roboflow
```

### Usage
1. Open `helmet_detection.ipynb` in Jupyter or Google Colab.
2. Follow the cells to:
   - Install dependencies.
   - Load the dataset (local or via Roboflow).
   - Train the YOLOv8 model.
   - Evaluate performance and run predictions.

## 🛠 Model Configuration
The notebook is configured to train a **YOLOv8 Nano (yolov8n.pt)** model by default, which is optimized for speed and efficiency.

```python
!yolo task=detect mode=train model=yolov8n.pt data=path/to/data.yaml epochs=25 imgsz=640
```

## 📊 Results and Visualization
Model outputs, including weights (`best.pt`) and performance graphs, are typically saved in the `runs/` directory. The notebook provides snippets to display prediction results directly.

---
*Developed for Vehicle and Worksite Safety Applications.*
