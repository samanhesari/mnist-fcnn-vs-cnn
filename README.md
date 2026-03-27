# MNIST: MLP vs CNN Comparison

## 🧠 Overview
This project compares the performance of a **Multilayer Perceptron (MLP)** and a **Convolutional Neural Network (CNN)** on the MNIST handwritten digit classification task.

The main goal is to understand how model architecture impacts performance on image data.

---

## 🎯 Objectives
- Build a **Multilayer Perceptron (MLP)** as a baseline model
- Build a **Convolutional Neural Network (CNN)**
- Train both models on the MNIST dataset
- Compare both models in terms of:
  - Accuracy
  - Loss performance
  - Training time
  - Generalization ability

---

## 📊 Dataset
- MNIST handwritten digit dataset
- 60,000 training images
- 10,000 test images
- Grayscale images (28×28 pixels)
- Classes: digits 0–9

---

## 🏗️ Model Architectures

### 🔹 Multilayer Perceptron (MLP)
- Input: Flattened 28×28 images (784 features)
- Fully connected dense layers
- Activation: ReLU
- Output: Softmax layer (10 classes)
- Loss function: Cross-entropy

### 🔹 Convolutional Neural Network (CNN)
- Convolutional layers for feature extraction
- ReLU activation
- MaxPooling layers for downsampling
- Fully connected dense layers
- Softmax output layer

---

## ⚙️ Tech Stack
- Python 🐍
- TensorFlow / Keras or PyTorch
- NumPy
- Matplotlib
- Jupyter Notebook (optional)

---

## 🚀 How to Run

```bash
git clone https://github.com/your-username/mnist-mlp-vs-cnn.git
cd mnist-mlp-vs-cnn
pip install -r requirements.txt