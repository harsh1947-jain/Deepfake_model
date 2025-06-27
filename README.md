# 🧠 Deepfake Detection using CNN-LSTM

A deep learning model that detects deepfake videos by leveraging spatial and temporal features using a hybrid CNN and LSTM architecture. The model was trained on the Celeb-DF dataset and achieved 86% accuracy.

---

## 📌 Features

- Combines **Convolutional Neural Networks (CNN)** for spatial feature extraction with **LSTM** for temporal sequence modeling.
- Trained on **200 real** and **200 fake** videos from the **Celeb-DF v2** dataset.
- Extracts **200 frames per video** and applies **real-time data augmentation**.
- Benchmarked against standard models like **VGG16** and **InceptionNet**.

---

## 📁 Dataset

- **Dataset**: [Celeb-DF v2]
- **Structure**: 200 real and 200 fake videos
- **Preprocessing**:
  - Extracted 200 frames per video
  - Converted frames to 240x240 resolution
  - Labeled fake = 0, real = 1

---

## 🧱 Architecture

- **CNN Backbone**: Custom 19-layer CNN or pre-trained VGG16 (optional)
- **LSTM**: Processes frame-level embeddings to capture temporal patterns
- **Classification**: Sigmoid layer for binary output (real vs fake)

---

## ⚙️ Training Details

- **Loss Function**: Binary Cross-Entropy
- **Optimizer**: Adam
- **Epochs**: 30
- **Validation Split**: 20%
- **Augmentation**: Flip, Rotation, Brightness, Zoom
- **Regularization**: Dropout and Batch Normalization

---

## 📊 Results

- **Accuracy**: **86%**
- **Improved generalization** using augmentation and regularization

![Final_Result](https://github.com/user-attachments/assets/5dd5419b-c2c3-4df5-918b-a11a94c54aed)







