# Acne Detection using YOLOv8

## 📌 Project Overview
This project develops an AI-based acne detection system using YOLOv8.  
The model detects acne regions on facial images and provides bounding box predictions for skincare analysis.

---

## 🧠 Model Details
- Model: YOLOv8m (Ultralytics)
- Task: Object Detection (Acne)
- Image size: 1024
- Training platform: Kaggle
- Optimizer: AdamW
- Epochs: 100

---

## 📊 Results
Final performance on validation/test dataset:

- Precision: **0.962**
- Recall: **0.883**
- mAP@0.5: **0.91**
- mAP@0.5:0.95: **0.703**

👉 The model achieves strong detection performance with high precision and good bounding box accuracy.

---

## 📁 Project Structure


acne-detection-project/
│
├── models/
│   └── acne_best.pt
│
├── metrics/
│   ├── confidence_curves.png
│   ├── confidence_sweep_metrics.csv
│   ├── metrics_summary.json
│   └── training_epoch_metrics.csv
│
├── results/
│   ├── results.png
│   ├── PR_curve.png
│   ├── F1_curve.png
│   ├── confusion_matrix.png
│
├── notebooks/
│   └── acne_training.ipynb
│
├── README.md
├── requirements.txt
└── .gitignore


#How to run 

from ultralytics import YOLO

model = YOLO("models/acne_best.pt")
model.predict("image.jpg")

#notes 


-use of public dataset on roboflow (all skin colors included, dataset not uploaded due to size )
Key Features
High precision detection (low false positives)
Good recall (detects most acne regions)
Improved mAP50-95 using augmentation techniques
Suitable for real-time skincare applications

Notes
Dataset is not included in the repository
Model trained and evaluated on Kaggle environment
Best model selected based on mAP50-95

👥 Team(from National donghwa University ) 

Medjina Agar Azor
Esperancia petit-frère
Sania Sael 
Deborah Asanterabi Ulomi