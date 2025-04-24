---
title: "EchoMotion"
excerpt: "Transformer-based Multi-View Cardiac Segmentation and EF Estimation from Echocardiography"
collection: portfolio
---

## 🫀 Project Overview

**EchoMotion** is a deep learning framework for automatic **left ventricle (LV) segmentation** and **ejection fraction (EF)** estimation from echocardiography videos. It combines **transformer-based encoders**, **temporal modeling**, and **multi-view learning** to approach expert-level accuracy in heart function analysis.

This project focuses on bringing **explainable AI** and **clinical alignment** to cardiac imaging by following physician-style EF estimation steps — **segmentation → volume → EF** — rather than direct regression.

---

## 🩺 Clinical Background

Ejection Fraction (EF) is a core indicator of cardiac function and is widely used in the diagnosis and monitoring of heart failure. Clinically, EF is calculated by measuring the change in **left ventricular (LV) volume** between **end-diastolic (ED)** and **end-systolic (ES)** frames of an echocardiography video.

Traditionally, this involves manually tracing the inner contour of the LV in two orthogonal views (A4C & A2C) — a time-consuming and operator-dependent process prone to variability.

Automating this process using deep learning not only accelerates analysis but also improves consistency. However, challenges include:

- Speckle noise and motion blur in ultrasound imaging  
- Anatomical variability  
- Generalization across different devices and patients

EchoMotion addresses these gaps by combining state-of-the-art segmentation models with clinical insight and multi-frame, multi-view input.

---

## 🎯 Research Objective

The goal of **EchoMotion** is to build an end-to-end deep learning framework for:

- Segmenting the **left ventricle (LV)** across all frames of an echocardiography video  
- Estimating **EF** using methods that are clinically aligned — via volume approximation rather than regression  
- Enhancing model **interpretability** with explainable outputs (e.g., Grad-CAM)  
- Improving **efficiency** through active learning and modular architecture

The focus is not just on model accuracy, but also on **trustworthiness**, **scalability**, and **realistic clinical deployment**.

---

## 🧠 Core Features

- **Transformer + U-Net Hybrid Architectures**  
  Custom segmentation models built on **SegFormer** backbone (B0–B2) enhanced with attention modules such as **SE**, **CBAM**, and **DANet**

- **Spatio-Temporal Frame Analysis**  
  Temporal context is leveraged using short frame sequences to improve cardiac cycle consistency and segmentation robustness

- **Multi-View Fusion (A4C + A2C)** *(in progress)*  
  Dual-encoder design with attention-based fusion for clinical biplane EF analysis

- **EF Estimation Pipeline**  
  EF is computed using **area-based volume approximations** over time, mirroring clinical Simpson’s method

- **Explainability via Grad-CAM**  
  Visual feedback on model attention improves interpretability for medical professionals

- **Active Learning Loop** *(planned)*  
  Integrates uncertainty-based sample selection to reduce annotation effort and improve label efficiency

---

## 🧪 Methodology

The pipeline consists of four core stages:

### 1. Preprocessing
- Frame-level decomposition of video sequences  
- Resizing and normalization (mean/std statistics)  
- Dataset split using official train/val/test partitions  

### 2. Segmentation Network (EchoMotionNet)
- Transformer-enhanced encoders: **SegFormer B0–B2**  
- U-Net style decoders with multi-scale skip connections  
- Attention modules: **SE**, **CBAM**, **DANet**  
- Optional sequence input for **temporal modeling**

### 3. Ejection Fraction Estimation
- **Area-based EF calculation**:  
  \[
  EF = \frac{EDV - ESV}{EDV} \times 100
  \]
- Frame-wise mask analysis to extract volume dynamics (ED/ES)  
- Optional regression head for joint segmentation + EF prediction  

### 4. Evaluation & Visualization
- Metrics: **Dice**, **IoU**, **MAE (EF)**, **R²**, **Pearson**  
- Visual outputs: predicted vs. ground truth masks, **EF scatter plots**  
- **Grad-CAM heatmaps** for model explainability

---

## 🛠️ Technologies Used

- **PyTorch** – for modeling and training  
- **Transformers** (HuggingFace + timm) – attention-based encoders  
- **Hydra** – for experiment configuration  
- **MLflow** – for experiment tracking and visualization  
- **OpenCV / PIL / Matplotlib** – for visualization  
- **Scikit-learn** – for evaluation metrics  

---

## 📊 Evaluation Highlights

- **Segmentation Metrics:** Dice, IoU  
- **EF Accuracy:** MAE, R², Pearson correlation  
- **Explainable Outputs:** Segmentation masks, Grad-CAM heatmaps, EF scatter plots  

---

## 💡 Why EchoMotion?

This project demonstrates:

- Practical experience in designing **modular, research-level deep learning pipelines**  
- Hands-on implementation of **Transformer architectures**, **temporal models**, and **active learning** workflows  
- The ability to **translate clinical workflows into AI logic**  
- A focus on **explainability and reproducibility**, which are essential in medical AI

---
