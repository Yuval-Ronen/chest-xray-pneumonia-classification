# Pneumonia Detection from Chest X-Ray Images
Deep Learning Final Project — Bar-Ilan University, 2024  
**Author:** Yuval Ronen

---

## 🩻 Project Overview
This project focuses on classifying chest X-ray images into **NORMAL** and **PNEUMONIA** categories using Convolutional Neural Networks (CNNs) and Transfer Learning techniques.  
The goal was to develop effective and efficient models capable of supporting diagnostic decision-making in medical imaging.

---

## 🎯 Key Features
- **Custom CNN Architecture:** Built and trained baseline convolutional models to establish initial performance.
- **Transfer Learning:** Fine-tuned pre-trained models including **VGG**, **ResNet152V2**, and **EfficientNetB0** for improved classification accuracy.
- **Model Iteration & Optimization:** Applied data augmentation, regularization, and batch normalization to reduce overfitting and improve generalization.
- **Performance Evaluation:** Systematically compared models to identify the best-performing architecture.

---

## 🧠 Approach

### 1) Baseline Model — Custom CNN
I began by developing a CNN from scratch to:
- Understand the feature representation needed
- Establish baseline performance
- Identify challenges such as overfitting

The custom CNN served as a **controlled starting point** for experimentation.

### 2) Transfer Learning Models
I then leveraged **pre-trained ImageNet models**, including:
- VGG
- ResNet152V2
- EfficientNetB0

These models were **fine-tuned** on the X-ray dataset.  
**EfficientNetB0 achieved the highest classification performance.**

### 3) Model Optimization Strategy
To improve generalization, I experimented with:
- Data augmentation (rotation, scaling, shifts)
- Dropout layers
- L1 / L2 Weight Regularization
- Batch Normalization
- Learning-rate adjustments and early stopping

This iterative process guided us to a **stable and high-performing final model**.

---

## 📊 Results Summary

| Model | Approach | Performance Summary |
|-------|---------|---------------------|
| Custom CNN | Baseline from scratch | Learned basic features but limited accuracy |
| VGG (Transfer Learning) | Moderate fine-tuning | Improved accuracy but prone to overfitting |
| ResNet152V2 (Fine-Tuned) | Trained last layers | Better representation learning |
| **EfficientNetB0 (Fine-Tuned)** | **Final model** | **Best performance and generalization** ✅ |

---

## 📂 Repository Structure
```bash
chest-xray-pneumonia-classification/
├── README.md
├── notebook/
│   └── chest-xray-pneumonia-classification.ipynb
└── images/       # (optional: example images)

---

---

## 🚀 How to Run
The notebook is already structured so that you can test the model **without re-training it**.

### 1) Open the Notebook in Google Colab
Open the project notebook here:  
https://colab.research.google.com/drive/1knkCV9MSnOlM0vU_9MSnES5mU3PtzSo5#scrollTo=2EBngprD0rip


### 2) Run the **Evaluation** Section Only
The **Evaluation** section:
- Loads the trained models directly from the notebook
- Runs predictions on test images
- Shows accuracy and sample outputs

✅ This allows you to test the model **immediately**, with **no training time**.

---

### 🧠 (Optional) Re-Training
If you want to retrain the model from scratch, run the section labeled **Training**.

> **Note:** Training takes **20–40 minutes** depending on GPU settings.  
For typical use and demonstration, **running Evaluation only is recommended.**

---

## 📎 Dataset
The dataset used in this project:  
https://www.kaggle.com/paultimothymooney/chest-xray-pneumonia

---

## 🙌 Acknowledgements
This project was completed as the final assignment for the **Deep Learning course at Bar-Ilan University (2024).**
