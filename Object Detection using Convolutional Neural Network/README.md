# Object Detection using Convolutional Neural Network

This project implements a Convolutional Neural Network (CNN) using TensorFlow/Keras to classify images from the **CIFAR-10** dataset.

## 📚 Dataset

- Dataset used: **CIFAR-10**
- Loaded using: `tensorflow.keras.datasets.cifar10`
- Consists of 60,000 32x32 color images in 10 different classes:
  - airplane, automobile, bird, cat, deer, dog, frog, horse, ship, truck

## 🔄 Preprocessing

- Images are normalized by dividing pixel values by 255.0 to scale them between 0 and 1.

## 🧠 Model Architecture

Constructed using `Sequential` model:

1. **Conv2D**: 32 filters, (3x3), ReLU, input shape (32, 32, 3)
2. **MaxPooling2D**: (2x2)
3. **Conv2D**: 64 filters, (3x3), ReLU
4. **MaxPooling2D**: (2x2)
5. **Conv2D**: 64 filters, (3x3), ReLU
6. **Flatten**
7. **Dense**: 64 units, ReLU
8. **Dense**: 10 units, Sigmoid (one for each class)

## 🛠 Tools & Libraries

- Python
- TensorFlow / Keras
- NumPy
- Matplotlib

## 🔍 Visualization

- Used `matplotlib.pyplot` to view sample images from the dataset

## 📝 Notes

- The model summary is printed after each major phase (convolutional + dense).
- The CNN is trained to perform **image classification** on CIFAR-10, not full object detection (i.e., no bounding boxes).

