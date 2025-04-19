# 🧠 Artificial Intelligence for Lumbar Spine Degenerative Classification

This repository contains the code and methodology for a deep learning-based diagnostic system that assists in the **detection and classification of lumbar spine degenerative conditions** using MRI data. The project aims to reduce diagnostic time and support radiologists in clinical decision-making.

## 🚀 Project Overview
Low back pain, often caused by spondylosis and disc degeneration, affects over 619 million people globally. MRI is vital for assessing these conditions but is time-consuming and labor-intensive. This project proposes an **AI-driven two-stage pipeline** to detect and classify five common spinal disorders across lumbar disc levels (L1/L2 to L5/S1) with severity levels (Normal, Mild, Moderate, Severe).

## 🛠️ Key Features
- **Stage 1: Localization**
  - 3D ConvNeXt model to identify instance numbers (MRI slice levels)
  - 2D CNN to predict precise (x, y) coordinates of vertebral disc levels

- **Stage 2: Severity Classification**
  - Uses image patches based on coordinates from Stage 1
  - MIL (Multiple Instance Learning) + Bi-LSTM for contextual analysis
  - Specialized preprocessing and augmentation for robustness

## 🧬 Target Conditions
- Left/Right Neural Foraminal Narrowing  
- Left/Right Subarticular Stenosis  
- Spinal Canal Stenosis

## 📊 Results
- Initial experiments show the model accurately localizes disc levels
- Promising results from visual and quantitative evaluations
- Confusion matrices and performance graphs included

## 🔮 Future Work
- Integrate severity scoring models
- Improve generalization with multi-task learning
- Finalize an end-to-end diagnostic pipeline ready for clinical use

