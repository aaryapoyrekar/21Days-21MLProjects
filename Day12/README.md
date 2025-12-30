# 🖼️ Image Super-Resolution using U-Net (32×32 → 128×128)

## 📌 Project Overview
This project implements an **image super-resolution system** using a **U-Net architecture**.  
The goal is to reconstruct a **high-resolution image (128×128)** from a **low-resolution input (32×32)**.

Super-resolution is a fundamental problem in computer vision, widely used in:
- Image enhancement
- Medical imaging
- Surveillance
- Photography and media restoration

---

## 🎯 Objective
- Input: **32 × 32 RGB image**
- Output: **128 × 128 RGB image**
- Learn a mapping that restores spatial details lost during downsampling

---

## 🧠 Why U-Net?
U-Net is well-suited for image-to-image tasks because:
- The **encoder** captures global context
- The **decoder** reconstructs spatial details
- **Skip connections** preserve fine-grained information

This makes U-Net effective for super-resolution problems.

---

## 🗂️ Dataset
- **CelebA Dataset**
- Images are:
  - Resized to **128×128** as ground truth
  - Downscaled to **32×32** as model input
- Pixel values normalized to `[0, 1]`

---

## 🏗️ Model Architecture
- Encoder–decoder U-Net
- Convolutional layers with Batch Normalization and ReLU
- MaxPooling for downsampling
- Transposed Convolutions for upsampling
- Extra upsampling layers to reach **128×128 resolution**
- Final `1×1` convolution to generate RGB output

---

## ⚙️ Training Configuration
- **Loss Function:** Mean Absolute Error (MAE)
- **Optimizer:** Adam
- **Batch Size:** 32
- **Training Strategy:** Generator-based training
- **Framework:** TensorFlow / Keras

---

## 📊 Results
- MAE loss decreases across epochs, indicating learning
- Visual inspection shows progressive improvement in image clarity
- Early predictions are blurry (expected) and improve with training

---

## 📈 Sample Outputs
Each epoch compares:
1. Original Image
2. Ground Truth (128×128)
3. Low-Resolution Input (32×32 → upscaled)
4. Model Prediction

This provides clear qualitative feedback on training progress.

---

## 🚀 How to Run
1. Load the CelebA dataset
2. Run cells sequentially:
   - Imports
   - Model definition
   - Data generator
   - Training
   - Visualization
3. Train the model and observe sample outputs

---

## 🔮 Future Improvements
- Use perceptual or SSIM loss
- Add adversarial training (SRGAN)
- Increase dataset diversity
- Train for more epochs
- Experiment with deeper architectures

---

## ✅ Conclusion
This project demonstrates that **U-Net can effectively perform image super-resolution**, converting low-resolution **32×32 images into high-resolution 128×128 outputs**.  
The results validate the power of encoder-decoder architectures for pixel-level reconstruction tasks.

---

## 👨‍💻 Author
**Aarya Poyrekar**  
Day 12 – 21 Days, 21 ML Projects
