# Breast Cancer Detection using Neural Network

This project implements a neural network using TensorFlow/Keras to classify whether a tumor is benign or malignant based on the Breast Cancer Wisconsin dataset.

## 📚 Dataset

- Dataset used: **Breast Cancer Wisconsin (Diagnostic) Dataset**
- Loaded using `sklearn.datasets.load_breast_cancer()`
- Features represent characteristics of cell nuclei in digitized images.

## 🔍 Data Preprocessing

- Converted dataset to a Pandas DataFrame
- Added the `target` column (0 = malignant, 1 = benign)
- Performed basic EDA: shape, data types, and value counts
- Used `StandardScaler` to normalize features

## 🧠 Model Architecture

- Built using `keras.Sequential` model
- Layers:
  - Flatten layer for input of shape (30,)
  - Dense layer with 20 neurons and ReLU activation
  - Dense output layer with 2 neurons and sigmoid activation

## ⚙️ Compilation

- Optimizer: `adam`
- Loss function: `sparse_categorical_crossentropy`
- Metrics: `accuracy`

## 🏋️ Model Training

- Trained the model for **20 epochs**
- Used 10% of the training data for validation during training

## 📊 Evaluation

- Plotted training and validation accuracy over epochs
- Plotted training and validation loss over epochs

## 📈 Prediction

- Predictions were made on the test set
- Used `np.argmax` to extract predicted classes from probability outputs

## 🛠 Tools & Libraries

- Python
- Pandas, NumPy, Matplotlib, Seaborn
- Scikit-learn
- TensorFlow / Keras
