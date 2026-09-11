# ✍️ Persian Handwritten Digit Recognition (From Scratch)

A custom **Multi-Layer Perceptron (MLP)** neural network implemented completely **from scratch using NumPy** for Persian handwritten digit recognition (0–9) on the **Hoda Dataset**.

---

## 📌 Project Overview
The goal of this project is to implement, train, and evaluate a deep learning classification pipeline from mathematical foundations without relying on high-level deep learning frameworks (like PyTorch or TensorFlow).

- **Dataset:** Hoda Persian Handwritten Digit Dataset (1,698 images)
- **Input Size:** 28 × 28 grayscale images (flattened to 784 features)
- **Target Classes:** 10 digits (۰ to ۹)
- **Train/Test Split:** 80% Train (1,358 samples) / 20% Test (340 samples)

---

## 🧠 Model Architecture & Details

| Parameter | Specification |
| :--- | :--- |
| **Model Type** | Multi-Layer Perceptron (MLP) from Scratch |
| **Input Layer** | 784 neurons (28x28 normalized pixels) |
| **Hidden Layer** | 64 neurons with **ReLU** activation |
| **Output Layer** | 10 neurons with **Softmax** activation |
| **Weight Initialization** | He Normal Initialization |
| **Loss Function** | Categorical Cross-Entropy |
| **Optimizer** | Gradient Descent (Learning Rate: `0.05`) |
| **Epochs** | 800 |

---

## 📊 Results & Performance

The model achieves solid convergence and generalization on unseen test data:

- **Test Accuracy:** `86.47%`
- **Macro Average F1-Score:** `0.87`
- **Weighted Average F1-Score:** `0.86`

### Detailed Classification Report
```text
precision    recall  f1-score   support

0       0.90      0.80      0.85        35
1       0.89      0.91      0.90        34
2       0.86      0.91      0.88        33
3       0.86      0.94      0.90        34
4       0.76      0.80      0.78        35
5       0.91      0.91      0.91        34
6       0.77      0.69      0.73        35
7       0.84      0.91      0.87        34
8       1.00      0.88      0.94        34
9       0.88      0.91      0.89        32

accuracy                           0.86       340

