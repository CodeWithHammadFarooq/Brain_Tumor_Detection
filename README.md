🧠 Brain Tumor Detection Using YOLOv10 🚀
This project is an advanced implementation of brain tumor detection from MRI scans using the YOLOv10 object detection algorithm. It leverages the power of deep learning, computer vision, and Roboflow-integrated datasets to accurately localize and identify brain tumors in medical images.

📌 Project Overview
Brain tumor detection is a critical task in the medical field. Timely and accurate diagnosis can greatly enhance the chances of effective treatment. This project automates that process using a cutting-edge object detection model—YOLOv10, the latest version in the YOLO family, known for its speed, efficiency, and real-time detection capabilities.

⚙️ Technologies Used
Python

YOLOv10 (You Only Look Once Version 10)

PyTorch

Ultralytics API

Google Colab

Roboflow

Gradio (for creating an interactive UI)

Matplotlib & OpenCV (for visualization)

🗃 Dataset
The dataset used was obtained from Roboflow, a platform that provides high-quality datasets tailored for deep learning. The specific dataset contains labeled brain MRI images categorized by the presence or absence of tumors. The annotations follow the YOLO format and were downloaded using the Roboflow Python API.

Classes: Tumor (single-class object detection)

Format: YOLOv8-compatible

Size: Includes training, validation, and test images

🧠 Model: YOLOv10
YOLOv10 is the latest innovation from the YOLO series, optimized for:

Real-time object detection

Low-latency deployment

High accuracy with small model sizes

We used the yolov10n.pt (nano version) as the base model for transfer learning. This makes the project lightweight and deployable on edge devices.

🔧 Workflow
Data Preparation:

Dataset imported using Roboflow

YOLO format applied

Model Training:

Training performed for 25–50 epochs

Evaluation metrics plotted (loss, precision, recall, mAP)

Prediction & Visualization:

Model used to predict tumors in unseen validation images

Results saved and visualized using matplotlib

Gradio App:

A user-friendly web interface created with Gradio

Users can upload MRI images and get real-time predictions

Annotated results shown instantly in the browser

📊 Results
The trained model showed impressive localization of tumors

Inference was fast and reliable even on Google Colab’s free tier

The Gradio app ensures accessibility for non-technical users

🌐 Future Improvements
Use larger YOLOv10 variants (yolov10s, yolov10m) for better accuracy

Integrate Flask/Django backend for real-world web deployment

Convert the model to ONNX/TFLite for mobile and embedded use

Extend the dataset to multi-class tumor classification (e.g., meningioma, glioma)

📽 Demo
The project includes:

Real-time detection notebook

Visual results for multiple images

Interactive Gradio demo for hands-on testing

