---
title: "EchoMotion"
excerpt: "Transformer-based Multi-View Cardiac Segmentation and EF Estimation from Echocardiography"
collection: portfolio
---

## 🫀 Project Overview

**EchoMotion** is a deep learning framework for automatic **left ventricle (LV) segmentation** and **ejection fraction (EF)** estimation from echocardiography videos. The model is built in two stages:

- First, a segmentation model is trained using only the **manually labeled ED and ES frames** (as provided in public datasets like EchoNet-Dynamic).
- Then, the model is used to generate segmentation masks for **all intermediate frames**, enabling full-sequence analysis and temporal learning.

This strategy allows us to **bootstrap a full cardiac cycle representation** from partial annotations — a practical approach in clinical datasets where dense labeling is expensive.

EchoMotion combines **transformer-based encoders**, **temporal modeling**, and **multi-view learning**, while preserving explainability and clinical alignment by mimicking expert workflows (segmentation → volume → EF).

---

## 🩺 Clinical Background

Ejection Fraction (EF) is a critical indicator of heart function, used to diagnose and monitor heart failure. Clinically, EF is calculated by measuring volume change of the **left ventricle (LV)** between **end-diastole (ED)** and **end-systole (ES)**.

This is usually done by manually tracing the LV in A4C and A2C echo views — a process that is slow, subjective, and prone to inter-observer variability.

Deep learning offers the potential to automate this process. However, challenges remain:
- Speckle noise and motion blur in ultrasound images  
- Anatomical variability between patients  
- Limited annotated data, typically only ED/ES frames per video  

EchoMotion addresses these challenges by combining **high-capacity segmentation models**, **temporal context**, and **view fusion** to produce a clinically relevant and scalable EF analysis system.

---

## 🎯 Research Objective

EchoMotion is designed to:

- Learn to segment the LV using only ED/ES-labeled frames  
- Automatically generate intermediate-frame masks across full cardiac cycles  
- Use those outputs to model **temporal dynamics** of heart motion  
- Estimate EF from derived volume curves using a clinical method  
- Support interpretability and trust via Grad-CAM and transparent calculations

This approach balances **clinical realism**, **data efficiency**, and **modern ML techniques**.

---

## 🧠 Core Features

- **Transformer + U-Net Hybrid Architectures**  
  Built on **SegFormer** backbones with integrated attention modules (SE, CBAM, DANet)

- **Sparse-to-Dense Learning Pipeline**  
  Trained on ED/ES pairs, generalized to full-sequence segmentation for full cardiac cycle modeling

- **Spatio-Temporal Frame Analysis**  
  Sequence modeling (planned) for smooth, consistent heart motion representation

- **Multi-View Fusion (in progress)**  
  Dual-encoder design to jointly leverage A4C and A2C views for improved EF estimation

- **Explainability via Grad-CAM**  
  Visualizes model attention to support clinical trust

- **Active Learning Loop (planned)**  
  Uses uncertainty-based selection to identify frames for further expert annotation

---

## 🧪 Methodology

The pipeline consists of four main stages:

### 1. Preprocessing
- Extract ED and ES labeled frames from echocardiography videos  
- Apply **CLAHE** for contrast enhancement and **bilateral filtering** to reduce speckle noise  
- Resize, normalize, and split into training/validation/test sets

### 2. Segmentation Network (EchoMotionNet)
- Encoder: **SegFormer B0–B2** backbones  
- Decoder: U-Net-style with skip connections  
- Attention: SE / CBAM / DANet modules  
- Trained only on ED/ES frames (sparse supervision)

### 3. Temporal Expansion & EF Estimation
- Use trained model to infer masks for **all frames** in the video  
- Compute LV area per frame, extract EDV/ESV, and calculate:
  
  \[
  EF = \frac{EDV - ESV}{EDV} \times 100
  \]
  
- (Planned) Learn temporal features directly using Bi-LSTM or Temporal Transformers

### 4. Evaluation & Visualization
- Metrics: Dice, IoU, MAE (EF), R², Pearson  
- Visual outputs: segmentation overlays, Grad-CAM maps, EF scatter plots

---

## 🛠️ Technologies Used

- **PyTorch**  
- **SegFormer** (via HuggingFace / Timm)  
- **Hydra** for configuration  
- **MLflow** for experiment tracking  
- **OpenCV**, **PIL**, **Matplotlib** for visualization  
- **Scikit-learn** for evaluation metrics

---

## 📊 Evaluation Highlights

- **Segmentation Metrics:** Dice, IoU  
- **EF Accuracy:** MAE, R², Pearson correlation  
- **Explainable Outputs:** Grad-CAM maps, EF area plots, segmentation overlays

---

## 💡 Why EchoMotion?

This project showcases:

- **Sparse-to-dense training strategies** for realistic clinical datasets  
- **Transformer-based architectures** in medical segmentation  
- **Temporal modeling potential** for dynamic anatomy  
- Strong focus on **explainability**, **clinical relevance**, and **future scalability**

---
