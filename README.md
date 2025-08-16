# 🚗🔒 Automatic License Plate Blurring System

[![Python](https://img.shields.io/badge/Python-3.8%2B-blue?logo=python)](https://www.python.org/)  [![PyTorch](https://img.shields.io/badge/PyTorch-2.6+-ee4c2c?logo=pytorch)](https://pytorch.org/)  [![YOLO](https://img.shields.io/badge/YOLO-v8%20%7C%20v10%20%7C%20v11-green?logo=github)](https://github.com/ultralytics/ultralytics)  [![YOLO](https://img.shields.io/badge/YOLOv8-Object%20Detection-green?logo=github)](https://github.com/ultralytics/ultralytics)  [![OpenCV](https://img.shields.io/badge/OpenCV-Image%20%26%20Video%20Processing-orange?logo=opencv)](https://opencv.org/)  [![Pandas](https://img.shields.io/badge/Pandas-Data%20Analysis-yellow?logo=pandas)](https://pandas.pydata.org/)  [![NumPy](https://img.shields.io/badge/NumPy-Numerical%20Computing-lightblue?logo=numpy)](https://numpy.org/)  [![Matplotlib](https://img.shields.io/badge/Matplotlib-Visualization-purple?logo=plotly)](https://matplotlib.org/)

Note: 📖 Please read the [Documentation](Automatic%20License%20Blurring.pdf) for more details.

This project is an **Automatic License Plate Blurring System** built using **YOLO object detection models**.  
The system detects license plates in both **images** and **videos**, then applies Gaussian blurring filter for privacy protection.  

---

## 📂 Dataset & Format

- **Source:** [Egyptian Cars Plates (Kaggle)](https://www.kaggle.com/datasets/mahmoudeldebase/egyptian-cars-plates)
  - 2,085 labelled images of Egyptian plates
- **Format:** `.csv`

---

## 📌 Features
- 🔍 **License Plate Detection** using YOLO
- 📊 **Model Performance Comparison** across different YOLO variants & training epochs
- 🏆 Selected the **best performing model** based on **Precision / Recall / mAP** metrics
- 🎥 **Real-world Application** on both images and videos
- 🔒 Automated **privacy preservation** by blurring detected plates

---

## 🧠 Model Training
1. Trained **YOLOv8n**, **YOLOv10n**, and **YOLOv11n** models with varying epochs (**3**, **5**, **10**)
2. Evaluated performance using:
   - ✅ Precision  
   - ✅ Recall  
   - ✅ mAP (Mean Average Precision)
   - ✅ Val_box_loss, Val_cls_loss, Val_cls_loss,
3. Selected the best-performing model (**YOLOv11n**) and trained it to **50 epochs**  
4. Used the final model on different **images & videos**

---

## 📊 Results
<img width="1742" height="414" alt="Precision" src="https://github.com/user-attachments/assets/a379988a-4a4f-4a65-bde2-f18b505ee10b" />
<img width="1743" height="414" alt="Recall" src="https://github.com/user-attachments/assets/e25d8a02-c5ee-491c-b8da-d911f5f219e9" />
<img width="1744" height="413" alt="mAP50" src="https://github.com/user-attachments/assets/f8ecc559-0cf1-4d69-8a04-56d0c42d16ab" />
<img width="1747" height="418" alt="mAP50-90" src="https://github.com/user-attachments/assets/62f6cb21-638c-42bd-a9a4-c5af2331381e" />
<img width="1744" height="413" alt="val_box_loss" src="https://github.com/user-attachments/assets/1a67ef2b-ffb4-495d-993c-c14a3f19ccce" />
<img width="1745" height="414" alt="val_cls_loss" src="https://github.com/user-attachments/assets/8e034e5b-f026-4a77-8a8f-cbb69e4963b1" />
<img width="1745" height="415" alt="val_dfl_loss" src="https://github.com/user-attachments/assets/60300d0a-baf0-4b00-b2bf-40def7c5522b" />

---

## 🖼️ Sample Results

<p align="center">
  <img src="https://github.com/user-attachments/assets/1d26c3d0-8229-4ae4-9fcf-b4d1f33d122b" alt="Before Blurring" width="45%"/>
  <img src="https://github.com/user-attachments/assets/f8eabb93-82c0-47b5-ace5-a2bb57012fdb" alt="After Blurring" width="45.5%"/>
  <img src="https://github.com/user-attachments/assets/fc369117-3b06-41d3-9299-6b807a3bc340" alt="After Blurring" width="45%"/>
  <img src="https://github.com/user-attachments/assets/e5789b8e-8d11-46d0-bd77-75d01dc5de44" alt="After Blurring" width="45%"/>
</p>

---
