 Handwritten Digit Recognition using MLP

 Problem Description
This project aims to build a Multilayer Perceptron (MLP) model to recognize handwritten digits (0–9) using the MNIST dataset.

---

 Dataset
The dataset used is the MNIST dataset.

🔗 Dataset Link:
http://yann.lecun.com/exdb/mnist/

- Total images: 70,000
- Image size: 28x28 pixels
- Classes: 10 digits (0–9)

---

 Data Preprocessing
- Normalized pixel values (0 → 255) to (0 → 1)
- Flattened images from 28x28 → 784 vector
- Converted labels using one-hot encoding

---

 🧠 Model Architecture (MLP)
- Input Layer: 784 neurons
- Hidden Layer 1: 128 neurons (ReLU)
- Hidden Layer 2: 64 neurons (ReLU)
- Output Layer: 10 neurons (Softmax)

---

s

 🔹 Experiment 1
- Activation: ReLU
- Neurons: 128 - 64

 🔹 Experiment 2
- Activation: Tanh
- Neurons: 256 - 128

---

  Results

| Experiment | Activation | Neurons | Accuracy | Loss |
|----------|----------|--------|---------|------|
| Exp 1 | ReLU | 128-64 | 0.9768 | 0.0905 |
| Exp 2 | Tanh | 256-128 | 0.9768 | 0.0804 |

---

 Analysis
- Both models achieved similar accuracy (~97.6%)
- Tanh achieved slightly lower loss
- Slight overfitting observed (train accuracy higher than validation)

---

 Techniques Used
- Dropout (0.3) to reduce overfitting

---

 How to Run

Install dependencies:# mlp-mnist-project
