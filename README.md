# Age and Gender Prediction from Images using CNN

This project implements a **Convolutional Neural Network (CNN)** to predict **age** and **gender** from facial images. The model is trained on the **UTKFace dataset** and can simultaneously estimate age and gender from a single image.

---

## Dataset

The dataset used is **UTKFace** (grayscale and color images of faces with age, gender, and ethnicity labels).

- **Kaggle link**: [UTKFace Dataset](https://www.kaggle.com/datasets/jangedoo/utkface-new)

---

## Features

- Multi-output CNN model for **simultaneous age and gender prediction**  
- Preprocessing: resizing to 128x128, grayscale conversion, normalization  
- Visualization of **training history**:
  - Accuracy and loss curves with difference lines
  - KDE plots for age distribution
  - Countplots for gender distribution  

---

## Model Architecture

- **Input**: 128x128 grayscale images  
- **Convolutional Layers**: 4 layers with increasing filters (32 → 256)  
- **Pooling**: MaxPooling after each convolution  
- **Dense Layers**: Two separate dense layers for age and gender  
- **Outputs**:  
  - Gender: sigmoid activation (probability)  
  - Age: ReLU activation (estimated age)  

---

## Usage

1. Clone the repository:
```bash
git clone https://github.com/karan89200/Age-and-Gender-Prediction-CNN-/tree/main
