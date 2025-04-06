---
title: "EchoMotion"
excerpt: "Deep learning-powered ejection fraction estimation from echocardiography videos"
collection: portfolio
---

## 🫀 Project Overview

**EchoMotion** is a deep learning project designed to automatically analyze heart function from echocardiography videos. By segmenting the **left ventricle (LV)** frame by frame, it estimates the **ejection fraction (EF)** — a key clinical metric of cardiac health.

The system mimics the clinical approach: identify **end-diastolic** and **end-systolic** frames, calculate area-based EF, and visualize the results — fully automated and explainable.

---

## 🩺 Clinical Background

- **Ejection Fraction (EF)** is a critical indicator of heart function.
- Current EF estimation is manual and subjective.
- EchoMotion automates this process, improving speed and reliability.
- Based on the widely-used **EchoNet-Dynamic** dataset by Stanford.

---

## 🎯 Research Objective

> Build a deep learning pipeline that segments the LV in echocardiography videos and calculates EF in an explainable way, following the same steps doctors do.

- Frame-wise **U-Net segmentation**
- Area change analysis for EF estimation
- Transparent and clinically aligned methodology

---

## 🧪 Methodology

**1. Preprocessing**
- Extracted and resized video frames (224×224)
- Normalization with dataset mean/std
- Dataset split into train/val/test

**2. Segmentation**
- Model: U-Net
- Loss: BCEWithLogitsLoss
- Optimizer: Adam
- Metrics: Dice Score, IoU

**3. EF Estimation**
- Compute LV area in all frames
- Find max (EDV) and min (ESV) areas
- Calculate EF: `(EDV - ESV) / EDV × 100`

**4. Evaluation & Visualization**
- Metrics: MAE, R², Pearson correlation
- Overlays and scatter plots for clarity

---

## 📊 Results

**Segmentation Accuracy**
- Dice: ~0.89
- IoU: ~0.82

**EF Prediction**
- MAE: ~4.2%
- R²: ~0.76
- Pearson: ~0.88

EchoMotion provides accurate and interpretable predictions. Visual outputs include EF curves and frame overlays for clinician trust.

---

## ⚙️ Tools Used

- **PyTorch**, **Hydra**, **Scikit-learn**
- **Matplotlib**, **Seaborn**
- Modular Python architecture with:
  - `data_generator.py`, `model_generator.py`, `trainer.py`, `predictor.py`

---

## 🚧 Challenges & Future Work

**Challenges**
- Noisy ground truth masks
- Motion blur in some frames
- No temporal modeling (frame-wise only)

**Future Work**
- Add temporal models (e.g., ConvLSTM, 3D CNN)
- Real-time EF estimation during live echo
- Extend to multi-view heart analysis

---

> 🧠 This project bridges deep learning and clinical cardiology to support faster, more objective heart function assessment.

---

