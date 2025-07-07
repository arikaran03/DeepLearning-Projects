# Digit Recognization using Convolutional Neural Network

This project implements a digit recognition model using a Convolutional Neural Network (CNN) trained on the MNIST dataset.

## Dataset

- The dataset used is **MNIST** which contains 70,000 grayscale images of handwritten digits (0 through 9).
- The data is preloaded from `tensorflow.keras.datasets`.

## Model Architecture

The Convolutional Neural Network used in this project consists of the following layers:

1. **Conv2D**: 32 filters, kernel size (3,3), activation ReLU
2. **MaxPooling2D**: pool size (2,2)
3. **Conv2D**: 64 filters, kernel size (3,3), activation ReLU
4. **MaxPooling2D**: pool size (2,2)
5. **Flatten**
6. **Dense**: 64 units, activation ReLU
7. **Dense**: 10 units, activation Softmax

## Preprocessing

- Normalization: pixel values are divided by 255.0
- Reshape input data to (28, 28, 1) to fit into the CNN
- Labels are one-hot encoded using `to_categorical`

## Training

- Optimizer: `adam`
- Loss function: `categorical_crossentropy`
- Metrics: `accuracy`
- Epochs: 5
- Batch size: 64

## Evaluation

- The model is evaluated on the test dataset using `model.evaluate()`.
- Metrics displayed include loss and accuracy.

## Model Saving

The trained model is saved using:
```python
model.save("digit_model.h5")
