# 🚗 Car Plate Detection and Recognition  

A computer vision project for **automatic license plate detection and recognition** using **YOLOv8** and an **End-to-End (E2E) recognition model**.  
The system detects car license plates in images and recognizes plate numbers with high accuracy.  

---

## 📌 Introduction
Automatic License Plate Recognition (ALPR) is widely applied in **traffic monitoring, parking management, and smart city systems**.  
This project combines **YOLOv8** for plate detection and an **E2E recognition model** for text extraction.  

---

## 📂 Dataset
- Car images with annotated license plates.  
- Preprocessed and split into `train/`, `val/`, and `test/`.  
- Applied augmentation (rotation, scaling, brightness) for robustness.  

---

## 🛠️ Technologies
- **Python 3.9+**  
- **YOLOv8 (Ultralytics)** – license plate detection  
- **OpenCV (cv2)** – image preprocessing  
- **E2E model** – end-to-end license plate recognition (`src/lp_recognition/E2E.py`)  
- **Collections.Counter** – statistical analysis of predictions  
- **time** – processing time measurement  

---

## 🚀 Workflow
1. **Detection**: YOLOv8 detects bounding boxes of license plates.  
2. **Recognition**: Extracted plates are passed to the **E2E recognition model** to decode text.  
3. **Analysis**: Count predictions with `Counter`, measure runtime with `time`.  

---

## 📊 Results
- Achieved reliable detection and recognition across test dataset.  
- Evaluated with **mAP, Precision, Recall, F1-score**.  
- Example:  

| Input Image | Detected Plate | Recognized Text |
|-------------|---------------|-----------------|
| 🚘 Car 1    | [Plate Box]   | 43A-12345       |
| 🚙 Car 2    | [Plate Box]   | 92B-67890       |

---

## ▶️ How to Run
```bash
git clone https://github.com/MinhHien2004/Car-Plate-Detect.git
cd ND+DKT_3/License-Plate-Recognition-master
python main_video9(tam_on).py
