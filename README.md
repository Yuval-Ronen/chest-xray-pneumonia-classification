# Pneumonia Detection from Chest X-Ray Images
Deep Learning Final Project — Bar-Ilan University, 2024  
**Authors:** Yuval Ronen & Mohammed Gara

---

## 🩻 Project Overview
This project focuses on classifying chest X-ray images into **NORMAL** and **PNEUMONIA** categories, and detecting pneumonia cases using **CNNs**, **transfer learning**, and **autoencoder-based anomaly detection**.

Our goal was to improve diagnostic support in medical imaging using deep learning techniques.

---

## 🎯 Key Features
- **Transfer Learning:** EfficientNetB0 & ResNet152V2 fine-tuned for medical image classification
- **Autoencoder for Anomaly Detection:** Achieved **~90.5% success rate**
- **Explainability:** Heatmap-by-Occlusion visualization to show what the model focuses on
- **GPU Training:** Implemented and trained on Google Colab (Tesla T4)

---

## 📂 Repository Structure
```
chest-xray-pneumonia-classification/
├── README.md
├── notebook/
│   └── chest_xray_project.ipynb
├── models/               # optional
└── images/               # example X-ray images + heatmaps
```

---

## 🧠 Models Used
| Model | Purpose | Notes |
|------|---------|------|
| EfficientNetB0 | Transfer Learning Classifier | Best classification performance |
| ResNet152V2 | Transfer Learning Classifier | Fine-tuned last 35 layers |
| Autoencoder (CNN-based) | Anomaly Detection | ~90.5% detection accuracy |

---

## 🔥 Explainability (Heatmap by Occlusions)
To highlight which lung regions influence the model's decisions, we generate heatmaps by sliding blackout windows over the image.

```
(images/heatmap_example_1.png)
(images/heatmap_example_2.png)
```

---

## 🚀 How to Run
### 1) Open the Notebook in Google Colab
```
notebook/chest_xray_project.ipynb
```

### 2) Enable GPU
```
Runtime → Change runtime type → GPU
```

### 3) Install dependencies
```
pip install tensorflow keras numpy matplotlib opencv-python
```

### 4) Run training or inference directly in the notebook.

---

## 📊 Results Summary
| Task | Accuracy | Method |
|------|---------|--------|
| Classification | ~94% | EfficientNet Transfer Learning |
| Anomaly Detection | ~90.5% | Autoencoder + MSE Thresholding |

---

## 📎 Links
- Dataset: https://www.kaggle.com/paultimothymooney/chest-xray-pneumonia
- Course: Deep Learning @ Bar-Ilan University

