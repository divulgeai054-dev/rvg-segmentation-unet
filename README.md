# 🦷 RVG Segmentation using UNet

<p align="center">
  <img src="https://img.shields.io/badge/Task-Image%20Segmentation-blue" />
  <img src="https://img.shields.io/badge/Model-UNet-green" />
  <img src="https://img.shields.io/badge/Framework-PyTorch-red" />
  <img src="https://img.shields.io/badge/Status-Active-success" />
</p>

---

## 📌 Overview

Dental Radiovisiography (RVG) images require precise pixel-level segmentation to identify anatomical structures and pathological regions.

This project builds a scalable UNet-based deep learning segmentation pipeline using a version-controlled experimental approach focused on dataset scaling, preprocessing, and model improvement.

---

## 📊 Dataset

- Total Images: 4459  
- Type: Grayscale Dental RVG scans  
- Task: Binary Segmentation  

| Version | Images | Description |
|--------|--------|-------------|
| v0.1   | 375    | Baseline experiment |
| v0.2   | 1047   | Improved training |
| v0.3   | 2953   | Large-scale training |
| Future | 4000+  | Full dataset |

---

## ⚙️ Preprocessing Pipeline

- Resize to 512 × 512  
- Normalize pixel values  
- Clean and align masks  
- Remove corrupted samples  
- Split: 80% Train / 10% Val / 10% Test  
- Progressive augmentation  

---

## 🧠 Model Development

### v0.1 — Baseline
- Standard UNet  
- Minimal preprocessing  
- No augmentation  

### v0.2 — Improved
- Increased dataset size  
- Improved training stability  
- Initial class imbalance handling  

### v0.3 — Scaled Training
- Dataset: 2953 images  
- Split: 80 / 10 / 10  

| Metric    | Score   |
|-----------|--------|
| Accuracy  | 0.7865 |
| Precision | 0.7936 |
| Recall    | 0.7865 |
| F1 Score  | 0.7874 |
| IoU       | 0.6757 |

---

## 🚀 Quick Start

### Clone Repository

```bash
git clone https://github.com/your-username/rvg-segmentation-unet.git
cd rvg-segmentation-unet
```
## ⚙️ Installation

### Install Dependencies
```bash
pip install -r requirements.txt
```
---
## ▶️ Run on Google Colab

| Version | Notebook | Open |
|--------|----------|------|
| v0.1 | 500 Images UNet Model | [![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1Bk2S5pE_igilmZFoZDiYyG76J7U12ro5?usp=sharing) |
| v0.2 | 1K Images UNet Model | [![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/10hVwpvi8G1vC5LiDQncKOqzPGMDOI3CX?usp=sharing) |
| v0.3 | 3K Images UNet Model | [![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1AmwJ96imPfmyIsTB6gzUeurZRfYIVugF?usp=sharing) |

---
## 💻 Run Locally

```bash
jupyter notebook
```
Open notebooks from the notebooks/ directory and update dataset paths accordingly.

---

## 📁 Project Structure

```bash
rvg-segmentation-unet/
│
├── notebooks/
│   ├── Preprocessing.ipynb
│   ├── 500 Images Unet Model.ipynb
│   ├── 1k-images-unet.ipynb
│   └── 3K_Unet_Model.ipynb
│
├── README.md
└── requirements.txt
```
---

## 📊 Evaluation Metrics

- Dice Coefficient  
- Intersection over Union (IoU)  
- Precision  
- Recall  
- F1 Score  

---

## 🚀 Roadmap

- Loss function optimization (Dice Loss, Focal Loss)  
- Segment Anything Model (SAM) comparison  
- Multi-class segmentation  
- Advanced architectures (Attention UNet, DeepLabV3+)  
- Full dataset training  

---

## ⚠️ Limitations

- Dataset still expanding  
- Label noise present  
- Limited augmentation in early versions  
- Binary segmentation only  

---

## 👨‍💻 Author

Divulge AI  

---

## ⭐ Highlights

- Version-controlled experimentation  
- Scalable training pipeline  
- Progressive dataset scaling  
- Designed for medical image segmentation workflows  
