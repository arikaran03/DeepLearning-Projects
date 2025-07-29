# 🧠 Breast Cancer Detection using Neural Network

This project helps detect breast cancer using a **Neural Network** built with **TensorFlow/Keras**. The model learns from a real-world dataset and predicts whether a tumor is **malignant (harmful)** or **benign (not harmful)**.

---
## 📌 What is this project about?

Breast cancer is one of the most common and serious diseases worldwide. This project uses a machine learning method called a **Neural Network** to classify tumors based on features like radius, texture, and smoothness.

The goal is to train the model to recognize patterns that indicate if a tumor is cancerous or not.

---
## 📚 Dataset Used

- **Name:** Breast Cancer Wisconsin (Diagnostic)
- **Source:** `sklearn.datasets.load_breast_cancer()`
- **Labels:**
  - `0` = Malignant (cancerous)
  - `1` = Benign (non-cancerous)

---

## ⚙️ Steps in the Project

### 1. Data Preprocessing
- **Convert to DataFrame:** Using Pandas for easy analysis
- **EDA:** Checked shape and class distribution
- **Scaling:** Used `StandardScaler()` to normalize feature values

### 2. Model Building
- **Framework:** TensorFlow / Keras
- **Model Type:** `Sequential`
- **Layers:**
  - `Flatten` → to reshape input (30 features)
  - `Dense(20)` with `ReLU` activation → hidden layer
  - `Dense(2)` with `sigmoid` → output layer

### 3. Compilation
- **Loss Function:** `sparse_categorical_crossentropy` → suitable for classification
- **Optimizer:** `adam` → adjusts learning rate
- **Metric:** `accuracy`

### 4. Training
- Trained for **20 epochs**
- Used **10%** of training data as validation set

### 5. Evaluation
- Plotted training and validation **accuracy** and **loss** using `matplotlib`

### 6. Prediction
- Used `model.predict()` to get probability values
- Applied `np.argmax()` to get the final class (0 or 1)

---

## 🛠️ Tools & Libraries

| Library         | Use                                      |
|----------------|-------------------------------------------|
| `pandas`       | DataFrame handling                        |
| `numpy`        | Numerical operations                      |
| `matplotlib`   | For plotting accuracy/loss                |
| `sklearn`      | Dataset loading & feature scaling         |
| `tensorflow.keras` | Building & training the neural network |

---


## ✅ Why Neural Networks?

Neural networks are used in many real-world applications like **medical diagnosis**, **image classification**, and **speech recognition**. They're good at learning complex relationships in data.

This project uses a basic feedforward neural network to detect breast cancer from patient data.

---

Feel free to explore and modify the code to improve predictions or try other models that are added in this repo!!

