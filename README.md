# Pneumonia Detection from Chest X-Ray Images
Deep Learning Final Project — Bar-Ilan University, 2024  
**Authors:** Yuval Ronen & Mohammed Gara

---

## 🩻 Project Overview
This project focuses on classifying chest X-ray images into **NORMAL** and **PNEUMONIA** categories using Convolutional Neural Networks (CNNs) and Transfer Learning techniques.  
Our goal was to develop effective and efficient models capable of supporting diagnostic decision-making in medical imaging.

---

## 🎯 Key Features
- **Custom CNN Architecture:** Built and trained baseline convolutional models to establish initial performance.
- **Transfer Learning:** Fine-tuned pre-trained models including **VGG**, **ResNet152V2**, and **EfficientNetB0** for improved classification accuracy.
- **Model Iteration & Optimization:** Applied data augmentation, regularization, and batch normalization to reduce overfitting and improve generalization.
- **Performance Evaluation:** Systematically compared models to identify the best-performing architecture.

---

## 🧠 Approach

### 1) Baseline Model — Custom CNN
We began by developing a CNN from scratch to:
- Understand the feature representation needed
- Establish baseline performance
- Identify challenges such as overfitting

The custom CNN served as a **controlled starting point** for experimentation.

### 2) Transfer Learning Models
We then leveraged **pre-trained ImageNet models**, including:
- VGG
- ResNet152V2
- EfficientNetB0

These models were **fine-tuned** on the X-ray dataset.  
**EfficientNetB0 achieved the highest classification performance.**

### 3) Model Optimization Strategy
To improve generalization, we experimented with:
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
