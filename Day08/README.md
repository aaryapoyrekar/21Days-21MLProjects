# 👗 Fashion-MNIST Image Classification using Deep Learning

## 📌 Project Overview
This project focuses on building and comparing multiple deep learning models to classify clothing images from the **Fashion-MNIST** dataset.  
The main objective is to analyze how **model architecture and complexity** impact performance on an image classification task.

Three models of increasing complexity were implemented and evaluated:
- Artificial Neural Network (ANN)
- Basic Convolutional Neural Network (CNN)
- Deeper CNN with Batch Normalization and Dropout

---

## 🧠 Key Learning Objectives
- Understand the limitations of ANN models for image data
- Learn how CNNs extract spatial features from images
- Compare shallow vs deeper CNN architectures
- Apply regularization techniques to control overfitting
- Analyze model behavior using confusion matrices and prediction visualization

---

## 📂 Dataset
- **Name:** Fashion-MNIST  
- **Images:** 28×28 grayscale images  
- **Classes:** 10 clothing categories  
- **Samples:**  
  - 60,000 training images  
  - 10,000 test images  

Each image represents a clothing item such as T-shirts, trousers, dresses, sneakers, bags, etc.

---

## 🔧 Data Preprocessing
- Pixel normalization (0–255 → 0–1)
- Reshaping images to include channel dimension `(28, 28, 1)`
- One-hot encoding of class labels
- Verification of dataset shapes before training

---

## 🏗️ Model Architectures

### 1️⃣ Artificial Neural Network (ANN)
- Flatten layer
- Fully connected dense layers
- Softmax output for multi-class classification  
**Purpose:** Baseline model for comparison

---

### 2️⃣ Basic CNN
- Convolution + MaxPooling layers
- Dense classifier
- Learns spatial patterns in images  
**Purpose:** Demonstrate advantage of CNNs over ANN

---

### 3️⃣ Deeper CNN
- Multiple convolution blocks
- Batch Normalization
- Dropout regularization
- Higher representational capacity  
**Purpose:** Test whether deeper models improve performance

---

## ⚙️ Model Training
- Optimizer: Adam  
- Loss Function: Categorical Crossentropy  
- Metrics: Accuracy  
- Callbacks:
  - Early Stopping
  - Model Checkpointing (best weights saved)

All models were trained using the same dataset split to ensure fair comparison.

---

## 📊 Model Evaluation
- Evaluation on unseen test data
- Comparison of loss and accuracy across models
- Training vs validation performance visualization
- Confusion matrices for class-wise performance analysis

---

## 🔍 Prediction Analysis
- Predictions generated using the best-performing model
- Visualization of:
  - Correctly classified images
  - Incorrectly classified images
- Helps understand common misclassifications and model limitations

---

## 🏆 Key Findings
- CNN models significantly outperformed the ANN model
- The **Basic CNN** achieved the best balance between accuracy and generalization
- The **Deeper CNN**, despite higher complexity, did not consistently outperform the Basic CNN
- Increasing complexity does not always guarantee better results

---

## ✅ Conclusion
This project demonstrates that:
- Convolutional Neural Networks are better suited for image classification tasks
- Moderate model complexity can outperform deeper architectures on simpler datasets
- Careful architecture selection is more important than blindly increasing depth

---

## 🛠️ Technologies Used
- Python
- TensorFlow / Keras
- NumPy
- Matplotlib
- Seaborn
- Plotly

