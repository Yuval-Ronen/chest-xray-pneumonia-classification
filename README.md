
# Pneumonia Detection from Chest X-Ray Images
Deep Learning Final Project — Bar-Ilan University (2024)  
**Author:** Yuval Ronen

## 🩻 Project Overview
This project focuses on classifying chest X-ray images into **NORMAL** and **PNEUMONIA** categories using Convolutional Neural Networks (CNNs) and **Transfer Learning**.  
The goal was to build effective diagnostic support models for medical imaging analysis.

## 🎯 Key Features
- **Custom CNN model** built as a baseline
- **Transfer Learning** using:
  - VGG
  - ResNet152V2
  - **EfficientNetB0 (Best Performing Model)**
- **Model optimization techniques** including:
  - Data augmentation
  - Dropout
  - L1/L2 weight regularization
  - Batch normalization
  - Learning rate scheduling + Early stopping
- **Direct evaluation without training** — run and test immediately

## 🧠 Methodology & Approach

### 1) Baseline CNN (Built From Scratch)
A custom CNN was implemented to:
- Understand the feature space
- Establish baseline accuracy
- Reveal overfitting trends and limits

### 2) Transfer Learning Experiments
We fine-tuned pre-trained ImageNet models:

| Model | Notes | Result |
|------|------|--------|
| VGG | Moderate fine-tuning | Improved, but unstable |
| ResNet152V2 | Trained last layers | Better feature extraction |
| **EfficientNetB0** | **Best performance** | ✅ Selected as final model |

### 3) Model Improvement Strategy
To improve classification accuracy:
- Applied **data augmentation** (rotations, flips, shifts)
- Added **dropout + L1/L2 regularization** to reduce overfitting
- Used **batch normalization** to stabilize gradients
- Tuned **learning rate + used EarlyStopping**

## 📊 Results Summary

| Model | Approach | Performance |
|------|---------|-------------|
| Custom CNN | Built from scratch | Learned basic structure, limited accuracy |
| VGG (Transfer Learning) | Partially fine-tuned | Better but inconsistent |
| ResNet152V2 | Fine-tuned last layers | Stronger representation |
| **EfficientNetB0** | **Fully fine-tuned** | **Best generalization & accuracy** ✅ |

## 📂 Repository Structure
```
chest-xray-pneumonia-classification/
├── README.md
└── notebook/
    └── chest_xray_project.ipynb
```

## 🚀 How to Run (No Training Needed)

### ✅ Open the Notebook in Google Colab
Run the project here:  
https://colab.research.google.com/drive/1knkCV9MSnOlM0vU_9MSnES5mU3PtzSo5#scrollTo=2EBngprD0rip

### ✅ Run **Evaluation** Section Only
This section:
- Loads the preconfigured models included in the notebook
- Runs prediction on the test dataset
- Displays accuracy, confusion matrix, and example outputs

**No training time is required.**
You get results immediately.

### 🧠 (Optional) Retraining
If desired, run the **Training** section in the notebook.  
Training time: *~20–40 minutes depending on GPU.*

## 📎 Dataset
Dataset used:  
https://www.kaggle.com/paultimothymooney/chest-xray-pneumonia

## 🙌 Acknowledgements
Project completed as part of the **Deep Learning Course** at **Bar-Ilan University (2024)**.
