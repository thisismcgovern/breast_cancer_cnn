
# 🧠 Breast Cancer Detection with CNN

This is a beginner-friendly CNN tutorial project where I trained a model to detect breast cancer from histopathology images.

## 🎯 Why This Project?

Breast cancer is one of the most common and deadly cancers in the world. Early and accurate diagnosis can save lives.  
This project explores how deep learning (specifically Convolutional Neural Networks) can assist in classifying biopsy images as **cancerous (malignant)** or **non-cancerous (benign)**.

I built this as a tutorial to learn how to:
- Handle real-world medical image datasets.
- Build and train CNNs from scratch using TensorFlow.
- Deal with imbalanced datasets and image classification workflows.

---

## 📁 Dataset

- **Source**: [Kaggle - Breast Histopathology Images](https://www.kaggle.com/datasets/paultimothymooney/breast-histopathology-images)
- Each image is 50x50 pixels.
- Organized into two classes:
  - `class0`: No cancer
  - `class1`: Cancer present

> ✅ After cleaning, ~198,000 benign and ~78,000 malignant images were used.

---

## 🏗️ Model Summary

A basic CNN was built using TensorFlow/Keras with the following layers:

```text
Input → Rescale → Conv2D + MaxPool → Conv2D + MaxPool → Conv2D + MaxPool → Flatten → Dense → Dropout → Sigmoid
