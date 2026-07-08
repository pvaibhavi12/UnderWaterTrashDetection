 
🌊 Underwater Trash Detection System using YOLOv5
📌 Overview

The Underwater Trash Detection System is a deep learning-based computer vision application that detects, localizes, and classifies underwater debris from images. The system leverages YOLOv5 for real-time object detection and provides an interactive Flask web application for image upload and visualization. To improve model transparency, SHAP and LIME are integrated for Explainable AI (XAI), enabling users to understand the model's predictions.

🚀 Features
Detects and localizes underwater trash using YOLOv5.
Classifies detected objects into three predefined categories.
Displays bounding boxes with confidence scores.
Real-time image inference through a Flask web interface.
Supports object counting and detection visualization.
Integrates SHAP and LIME for model explainability.
Trained and evaluated using Precision, Recall, and mAP metrics.
🛠️ Tech Stack
Programming Language: Python
Deep Learning Framework: YOLOv5 (PyTorch)
Computer Vision: OpenCV
Web Framework: Flask
Explainable AI: SHAP, LIME
Environment: Google Colab
Dataset: Kaggle Underwater Trash Detection Dataset
📂 Project Structure
Underwater-Trash-Detection/
│── dataset/
│   ├── train/
│   ├── val/
│   └── test/
│
│── runs/
│   └── detect/
│       └── train/
│           └── weights/
│               ├── best.pt
│               └── last.pt
│
│── app.py
│── detect.py
│── requirements.txt
│── README.md
│── data.yaml
📊 Dataset

The model was trained using an annotated underwater trash detection dataset obtained from Kaggle.

Dataset Split
Dataset	Images
Train	5720
Validation	820
Test	1144

Total Images: 7684

Each image is accompanied by a YOLO-format annotation file containing the object class and bounding box coordinates.

⚙️ Model Architecture

The project uses YOLOv5, a one-stage object detection model consisting of:

Backbone: Feature extraction
Neck: Multi-scale feature aggregation
Detection Head: Bounding box regression, object classification, and confidence prediction
📈 Training
Model: YOLOv5
Epochs: 10
Optimizer: SGD (default YOLOv5)
Framework: PyTorch
Evaluation Metrics
Precision
Recall
mAP@50
mAP@50-95
🖥️ Flask Application

The Flask web application enables users to:

Upload underwater images.
Perform real-time object detection.
Display detected objects with bounding boxes.
Visualize prediction results and object counts.
🔍 Explainable AI (XAI)

To improve transparency and interpretability, the project integrates:

SHAP (SHapley Additive exPlanations): Highlights the image regions that contribute most to a prediction.
LIME (Local Interpretable Model-agnostic Explanations): Explains individual predictions by identifying the most influential regions of an image.

📌 Future Enhancements
Support additional underwater trash categories.
Improve detection accuracy using larger datasets.
Enable real-time video and live camera detection.
Deploy the application on cloud platforms.
Add pollution analytics and reporting dashboards.
📷 Sample Output
Upload an underwater image.
Detect trash objects with bounding boxes.
Display confidence scores and object counts.
Visualize SHAP/LIME explanations for model predictions.

Individual Project


⭐ Key Skills Demonstrated
Deep Learning
Computer Vision
Object Detection
YOLOv5
PyTorch
OpenCV
Flask
Explainable AI (SHAP & LIME)
Model Evaluation
Google Colab
Kaggle API
