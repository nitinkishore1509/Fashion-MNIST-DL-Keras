# 🧥 Fashion MNIST Classification with Deep Learning (Keras)

This repository contains a deep learning project for **image classification** using the [Fashion-MNIST dataset](https://github.com/zalandoresearch/fashion-mnist).  
The project is implemented in **Python** using **TensorFlow/Keras**, demonstrating the use of Convolutional Neural Networks (CNNs) to classify grayscale fashion images into 10 categories.

---

## 📌 Project Overview
Fashion-MNIST is a drop-in replacement for MNIST, consisting of 70,000 grayscale images in 10 categories.  
Each image is **28x28 pixels** and represents items like shoes, t-shirts, dresses, and more.

In this project, we:
- Load and preprocess the dataset
- Build a deep learning model using **Keras Sequential API**
- Train and evaluate the model
- Visualize training history and predictions

---

## 📊 Dataset
The dataset contains the following **10 classes**:

| Label | Class Name         |
|-------|--------------------|
| 0     | T-shirt/top        |
| 1     | Trouser            |
| 2     | Pullover           |
| 3     | Dress              |
| 4     | Coat               |
| 5     | Sandal              |
| 6     | Shirt               |
| 7     | Sneaker             |
| 8     | Bag                 |
| 9     | Ankle boot          |

**Data split**:
- Training set: **60,000 images**
- Test set: **10,000 images**

---

## 🛠 Model Architecture
The CNN model was built using **Keras** and consists of:

- **Conv2D** layers with ReLU activation
- **MaxPooling2D** layers for downsampling
- **Dropout** for regularization
- **Flatten** + Dense layers for classification
- Output layer with **softmax** activation (10 classes)

Example architecture:

Conv2D → ReLU → MaxPooling2D → Dropout

Conv2D → ReLU → MaxPooling2D → Dropout

Flatten → Dense(128) → ReLU → Dropout → Dense(10, softmax)


---

## 📈 Training & Evaluation
- **Loss function**: `categorical_crossentropy`
- **Optimizer**: `adam`
- **Metrics**: `accuracy`
- **Epochs**: 10 (modifiable)
- **Batch size**: 128

---

**Final Performance (Test set)**:
| Metric        | Value  |
|---------------|--------|
| Accuracy      | 93.35% |
| Loss          | 0.1849 |

---
