# 🦷 RVG Segmentation using UNet

## 📌 Problem Statement
Dental RVG (Radiovisiography) images require precise pixel-level segmentation for identifying anatomical structures and lesions. Manual annotation is time-consuming and error-prone.

This project aims to build a robust deep learning-based segmentation pipeline using UNet, improving performance across increasing dataset scales and preprocessing strategies.

---

## 📊 Dataset

- **Total Images Available:** 4459  
- **Image Type:** Grayscale Dental RVG scans  
- **Task:** Image Segmentation  

### 📂 Dataset Usage by Version

| Version | Dataset Size | Description |
|--------|------------|-------------|
| v0.1   | 375 images  | Initial baseline experiment |
| v0.2   | 1047 images | Improved training with more data |
| Future | 4000+ images | Scaling phase (ongoing) |

---

## ⚙️ Data Preprocessing Pipeline

The preprocessing pipeline ensures consistency and improves model performance.

### Steps:
- Resize images to **512 × 512**
- Convert to grayscale (if required)
- Normalize pixel values
- Align and clean segmentation masks
- Remove corrupt or inconsistent data
- Apply augmentations (in later versions)

### Files:
- `Preprocessing.ipynb`
- preprocessing scripts (planned modularization)

---

## 🧠 Model Development (Versioned)

### 🔹 v0.1 — Baseline UNet
- Dataset: 375 images  
- Standard UNet architecture  
- Basic preprocessing  
- No heavy augmentation  

**Objective:** Establish baseline performance  

---

### 🔹 v0.2 — Improved UNet
- Dataset: 1047 images  
- Increased dataset size  
- Improved training stability  
- Initial class imbalance handling  

**Objective:** Improve generalization  

---

### 🔹 Upcoming Versions
- v0.3: Data augmentation strategies  
- v0.4: Class-weighted loss tuning  
- v0.5: SAM (Segment Anything Model) comparison  
- v1.0: Training on full dataset (4000+ images)  

---

## 📁 Project Structure
```
rvg-segmentation-unet/
│
│
├── notebooks/
│ ├── Preprocessing.ipynb
│ ├── 500 Images Unet Model.ipynb
│ └── 1k-images-unet.ipynb
│
│
├── README.md
└── requirements.txt 
```
---

## 📈 Training Strategy

- Progressive dataset scaling  
- Iterative model improvements  
- Validation-based monitoring  
- Focus on improving generalization  

---

## 📊 Evaluation Metrics

- Dice Coefficient  
- Intersection over Union (IoU)  
- Precision  
- Recall  

---

## 🚀 Future Work

- Integration with Segment Anything Model (SAM)  
- Multi-class segmentation  
- Advanced architectures (DeepLabV3, Attention UNet)  
- Full dataset training  
- Benchmarking across multiple models  

---

## 🔗 Planned Extensions

This project is part of a larger system:

- UNet → Current repository  
- SAM → Upcoming repository  
- Benchmark → Comparative analysis across models  

---

## ⚠️ Current Limitations

- Dataset still expanding  
- Limited augmentation in early versions  
- Code not fully modular (work in progress)  
- SAM integration pending  

---

## 👨‍💻 Author
Divulge AI
---

## ⭐ Key Highlight

This project follows a versioned experimental approach, progressively improving segmentation performance with increasing dataset size and refined preprocessing strategies, similar to real-world ML system development.
