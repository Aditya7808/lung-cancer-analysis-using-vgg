# 🩺 Lung Cancer Detection using Deep Learning

This repository contains a deep learning-based solution for the **automatic detection of lung cancer** from medical imaging data (such as CT scans or X-ray images). Lung cancer is a leading cause of cancer-related deaths worldwide, and early detection can significantly improve survival rates. This project leverages **Convolutional Neural Networks (CNNs)** to accurately classify lung images as cancerous or non-cancerous.

> **Note**: This project is a fork of [`badri0412/Lung_Cancer`](https://github.com/badri0412/Lung_Cancer) and has been **significantly enhanced with better structure, visualization, model evaluation, and documentation**.

---

## 🧠 Project Description

The goal of this project is to build a robust, efficient, and interpretable model to assist radiologists and medical professionals in detecting lung cancer at an early stage. Here's a breakdown of the core elements:

### 🎯 Objectives

- Automate lung cancer classification using deep learning
- Build an intuitive training pipeline for reproducibility
- Ensure scalability for real-world deployment
- Achieve high accuracy while minimizing false negatives (very critical in medical diagnosis)

### 📊 Approach

- Use a CNN-based architecture trained on lung CT or X-ray image datasets
- Perform preprocessing (resizing, normalization) and data augmentation to reduce overfitting
- Evaluate model using classification metrics (accuracy, precision, recall, F1 score)
- Visualize predictions and loss/accuracy graphs
- Build a modular and easy-to-understand codebase

---

## 📁 Dataset

- **Source**: Public datasets from [Kaggle](https://www.kaggle.com/datasets) and similar platforms
- **Structure**:
  - `/data/train/0` – Images without lung cancer
  - `/data/train/1` – Images with lung cancer
- **Size**: Varies depending on dataset chosen
- **Preprocessing**:
  - Grayscale conversion (if needed)
  - Image resizing to 224x224
  - Normalization to [0, 1] range

---

## 🧰 Model Architecture

The model is a **custom CNN** designed for binary image classification. Key components include:

- 3–4 Convolutional layers (with ReLU activations and BatchNorm)
- MaxPooling layers to downsample features
- Dropout for regularization
- Fully Connected Dense layers
- Sigmoid activation in the final layer for binary classification

> Optimizer: `Adam`  
> Loss Function: `BinaryCrossentropy`  
> Evaluation: Accuracy, Precision, Recall, F1-Score

---

## ⚙️ Installation

```bash
# Clone the repo
git clone https://github.com/Aditya7808/Lung_Cancer_Detection.git
cd Lung_Cancer_Detection

# Install dependencies
pip install -r requirements.txt
