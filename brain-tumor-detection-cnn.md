# 🧠 Brain Tumor Detection using Deep CNNs (94% Accuracy)

## 🚀 Overview

Medical image analysis is one of the most impactful applications of Deep Learning.  
In this project, I built a **Convolutional Neural Network (CNN)** model to detect brain tumors from MRI scans with high accuracy.

The goal was to assist in early diagnosis by automating the classification process.

---

## ❗ Problem Statement

Manual diagnosis of brain tumors from MRI images:

- Requires expert radiologists  
- Time-consuming and subjective  
- Risk of human error in early-stage detection  

👉 Goal:
Build a model that can **automatically classify MRI images** as tumor / no tumor with high accuracy.

---

## ⚙️ Approach & Solution

I used **Deep Learning with Transfer Learning** to build a high-performance model.

### 🛠 Tech Stack

- Python
- TensorFlow / Keras
- OpenCV
- NumPy, Pandas
- Matplotlib

---

### 🧩 Model Architecture

I leveraged **VGG16 (pretrained CNN)** and fine-tuned it for this classification task.
│
▼
Pretrained VGG16 Layers
│
▼
Fully Connected Layers
│
▼
Dropout (Regularization)
│
▼
Output Layer (Softmax)


---

### 🔍 Key Steps

#### 1. Data Preprocessing
- Resized MRI images to fixed dimensions  
- Normalized pixel values  
- Applied data augmentation:
  - Rotation  
  - Flipping  
  - Zoom  

#### 2. Transfer Learning
- Used **VGG16 pretrained on ImageNet**
- Froze initial layers
- Fine-tuned deeper layers for domain-specific learning

#### 3. Training
- Loss Function: Categorical Crossentropy  
- Optimizer: Adam  
- Evaluation: Accuracy, Loss curves  

#### 4. Evaluation
- Achieved **~94% accuracy** on validation data  
- Reduced overfitting using dropout and augmentation  

---

## 📊 Results

- ✅ Accuracy: **94%**
- ✅ Robust performance on unseen MRI images  
- ✅ Reduced need for manual inspection  

---

## 🧩 Challenges Faced

- Limited labeled medical dataset  
- Overfitting in early stages  
- Need for careful hyperparameter tuning  
- Handling class imbalance  

---

## 💡 Key Learnings

- Transfer Learning saves massive training time  
- Data augmentation is critical for small datasets  
- CNNs are powerful for image-based problems  
- Model interpretability is important in healthcare  

---

## 🚀 Future Improvements

- Use advanced architectures (ResNet, EfficientNet)  
- Add Grad-CAM for model explainability  
- Deploy as a web app for real-time predictions  
- Train on larger medical datasets  

---

## 🙌 Final Thoughts

This project gave me hands-on experience in applying **Deep Learning to real-world healthcare problems**.  
It strengthened my understanding of **CNNs, transfer learning, and model optimization**.
