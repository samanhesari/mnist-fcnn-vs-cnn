# MNIST: MLP vs CNN Comparison

## 🧠 Overview
This project compares the performance of a **Multilayer Perceptron (MLP)** and a **Convolutional Neural Network (CNN)** on the MNIST handwritten digit classification task.

The goal is to understand how different neural network architectures perform on image classification problems.

---

## 🎯 Workflow (What to Do)

1. Load MNIST dataset  
2. Visualize sample images  
3. Build models (MLP and CNN)  
4. Train both models  
5. Evaluate models on training and test sets  
6. Compare results (accuracy)  
7. Visualize predictions and performance  

---

## 📊 Dataset
- MNIST handwritten digit dataset  
- 60,000 training images  
- 10,000 test images  
- Grayscale images (28×28 pixels)  
- 10 classes: digits 0–9  

---

# 🏗️ Model Architectures

## 🔹 Multilayer Perceptron (MLP)

A fully connected neural network that processes flattened image inputs.

### 📌 Architecture
- Input: Flattened 28×28 images (784 features)  
- Fully connected dense layers  
- Activation: ReLU  
- Output: Softmax (10 classes)  
- Loss: Cross-entropy  

### 📊 Details
- Trainable layers: 3  
- Total parameters: 443,610  
- No spatial feature extraction (fully connected network)

---

## 🔹 Convolutional Neural Network (CNN)

A deep learning model designed for image data using convolution operations.

### 📌 Architecture
- Convolutional layers for feature extraction  
- ReLU activation  
- MaxPooling layers for downsampling  
- Fully connected dense layers  
- Softmax output layer  

### 📊 Details
- Trainable layers: 6  
- Total parameters: 421,834  
- Learns spatial patterns (edges, curves, shapes)

---

## 🔍 Architecture Difference

- **MLP** flattens images into 1D vectors → loses spatial information  
- **CNN** preserves 2D structure → learns spatial features  
- CNN is more suitable for image classification tasks  

---

# 📊 Results Comparison

## ✅ Accuracy Table

| Model | Training Accuracy | Test Accuracy |
|------|------------------|--------------|
| MLP  | 1.00 (100%)      | 0.98 (98%)   |
| CNN  | 1.00 (100%)      | 0.99 (99%)   |

---

## 📌 Results Summary
CNN outperforms MLP due to its ability to capture spatial features such as edges and strokes in handwritten digits. This allows CNN to better understand the structure of images, leading to improved generalization performance on unseen data compared to MLP.

---

## ⚙️ Tech Stack
- Python 🐍  
- TensorFlow / Keras or PyTorch  
- NumPy  
- Matplotlib  
- Scikit-learn  
- Jupyter Notebook  

---

## 🚀 How to Run

```bash
git clone https://github.com/your-username/mnist-mlp-vs-cnn.git
cd mnist-mlp-vs-cnn
pip install -r requirements.txt