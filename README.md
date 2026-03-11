# 🦴 Deep Learning-Based Grading of Knee Osteoarthritis

A deep learning system for **automatic grading of Knee Osteoarthritis (OA)** using knee X-ray images.  
The model predicts disease severity based on radiographic features using **convolutional neural networks and transfer learning**.

This project aims to assist **early diagnosis and severity assessment** of osteoarthritis in clinical settings.

---

# 📌 Problem Statement

Knee osteoarthritis (OA) is a degenerative joint disease that affects millions of people worldwide.  
Traditional grading methods rely on **manual interpretation of X-rays by radiologists**, which can be:

- Time consuming
- Subjective
- Prone to inter-observer variability

This project builds a **deep learning model to automatically classify OA severity from knee X-ray images**.

---

# 🧠 Model Overview

The system uses **transfer learning with deep convolutional neural networks** to extract meaningful radiographic features.

### Architecture

Dual-output CNN architecture with:

- **Backbone Networks**
  - ResNet
  - EfficientNet

- **Outputs**
  - KL Grade prediction
  - Ahlback Grade prediction
  - OA severity classification

---

# 📊 Dataset

- Dataset Size: **9,786 X-ray images**
- Image Type: **Knee Radiographs**
- Classification: **5 Classes**

| Class | KL Grade | Description |
|------|------|------|
| 0 | Normal | No signs of OA |
| 1 | Doubtful | Minor osteophyte formation |
| 2 | Mild | Definite osteophytes |
| 3 | Moderate | Joint space narrowing |
| 4 | Severe | Severe degeneration |

Dataset split:

Images are organized into class folders.

---

# ⚙️ Technologies Used

| Category | Tools |
|--------|--------|
Programming | Python |
Deep Learning | PyTorch |
Models | ResNet, EfficientNet |
Image Processing | OpenCV |
Data Handling | NumPy, Pandas |
Visualization | Matplotlib, Seaborn |
Model Explainability | Score-CAM |

---

# 🧪 Training Pipeline

The pipeline includes:

1️⃣ Data preprocessing  
2️⃣ Image augmentation  
3️⃣ Transfer learning with pretrained CNNs  
4️⃣ Hyperparameter tuning  
5️⃣ Model evaluation

Training techniques:

- Transfer Learning
- Class-balanced sampling
- Data augmentation
- Early stopping

---

# 📈 Model Performance

| Metric | Score |
|------|------|
Accuracy | **72%**
Macro F1 Score | **0.73**

Evaluation metrics used:

- Accuracy
- Precision
- Recall
- F1-score
- Confusion Matrix

---

# 🔍 Model Explainability

To ensure clinical interpretability, the model integrates:

### Score-CAM

Score-CAM visualizations highlight **important regions of X-rays** that influence predictions.

This helps verify that the model focuses on:

- Joint space
- Osteophytes
- Bone structures


