# 🥔 Potato Leaf Disease Classification with CNN

This project implements a Convolutional Neural Network (CNN) using TensorFlow and Keras to classify potato leaf images into three categories:

* **Potato\_\_\_Early\_blight**
* **Potato\_\_\_Late\_blight**
* **Potato\_\_\_healthy**

## 📁 Dataset

The dataset used is structured in three subdirectories, one for each class:

```
potato-dataset/
├── Potato___Early_blight/
├── Potato___Late_blight/
└── Potato___healthy/
```

Images are automatically loaded and split into training, validation, and test sets.

---

## 🧠 Model Architecture

The model uses a deep CNN architecture with the following key layers:

* **Image Preprocessing**:

  * Resizing to 256×256
  * Rescaling pixel values (1./255)
  * Data augmentation (flips and rotations)

* **Convolutional Layers**:

  * 6 Conv2D layers with ReLU activation
  * MaxPooling after each convolution block

* **Dense Layers**:

  * Flatten → Dense(64) → Dense(3) with softmax

---

## ⚙️ Training Configuration

* **Image size**: 256x256
* **Batch size**: 32
* **Epochs**: 20
* **Optimizer**: Adam
* **Loss Function**: Sparse Categorical Crossentropy
* **Metrics**: Accuracy

---

## ✅ Results

* **Test Accuracy**: **\~97.84%**
* Model performs well with clear distinction between the three classes.
---

## 📌 Requirements

* TensorFlow 2.x
* NumPy
* Matplotlib
---


