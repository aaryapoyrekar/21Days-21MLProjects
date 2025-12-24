# 🔍 Transfer Learning for Image Classification (CIFAR-100)

## 📌 Project Overview
This project demonstrates the use of **transfer learning** with pre-trained Convolutional Neural Networks (CNNs) for multi-class image classification on the **CIFAR-100 dataset**.

Instead of training deep neural networks from scratch, the project leverages models pre-trained on **ImageNet** to reuse powerful feature extractors and adapt them to a new task with 100 fine-grained classes. The goal is to compare how different architectures perform under similar conditions.

---

## 🎯 Objectives
- Understand and apply transfer learning in computer vision
- Compare popular pre-trained CNN architectures
- Analyze the effect of model depth and complexity
- Practice freezing and fine-tuning strategies
- Build intuition for selecting models in real-world vision tasks

---

## 🧠 Models Used
- **ResNet50**
- **VGG16**
- **MobileNetV2**

Each model was:
- Loaded without its top classification layer
- Extended with a custom classification head
- Fine-tuned selectively to adapt to CIFAR-100

---

## 🗂 Dataset
**CIFAR-100**
- 60,000 RGB images (32×32)
- 100 object categories
- Balanced class distribution
- More challenging than CIFAR-10 due to fine-grained labels

---

## ⚙️ Project Workflow

### 1. Data Loading & Preprocessing
- Loaded CIFAR-100 using TensorFlow
- Applied model-specific preprocessing
- Maintained a consistent training pipeline for fair comparison

### 2. Model Adaptation
- Removed original ImageNet classifier
- Added Global Average Pooling
- Added dense layers for 100-class prediction

### 3. Training & Fine-Tuning
- Trained models with frozen base layers
- Partially unfroze top layers for fine-tuning
- Used short training runs to compare convergence behavior

### 4. Evaluation & Comparison
- Evaluated all models on the test set
- Compared accuracy and learning stability

---

## 📊 Results Summary

| Model         | Test Accuracy |
|--------------|---------------|
| **ResNet50** | **~44%** |
| VGG16        | ~23% |
| MobileNetV2  | ~20% |

**Insight:**  
Deeper architectures with residual connections generalize better on complex datasets like CIFAR-100.

---

## 🧩 Key Learnings
- Transfer learning significantly reduces training time
- Model architecture strongly impacts performance
- Preprocessing must match the pre-training setup
- Fine-tuning only higher layers often yields better results
- Lightweight models trade accuracy for efficiency

---

## 🛠 Tech Stack
- Python
- TensorFlow / Keras
- NumPy
- Matplotlib
- Google Colab

---

## 📁 Saved Models
- `resnet50_cifar100.h5`
- `vgg16_cifar100.h5`
- `mobilenetv2_cifar100.h5`

---

## 🚀 Future Improvements
- Add data augmentation
- Tune learning rate schedules
- Visualize misclassified samples
- Experiment with EfficientNet and Vision Transformers

---

## 📌 Part of Series
**21 Days | 21 Machine Learning Projects**  
A hands-on journey from ML fundamentals to advanced deep learning.
