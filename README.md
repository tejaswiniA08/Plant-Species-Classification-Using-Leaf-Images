
# 🌿 Plant Species Classification using Leaf Images

This project focuses on automating the classification of plant species using deep learning models trained on leaf image features. It leverages the **One Hundred Plant Species Leaves Dataset** from the UCI Machine Learning Repository, aiming to aid botanists and researchers in accurate, fast, and scalable plant identification.

🔗 **Dataset Link**: [UCI Repository - Plant Species Leaves Dataset](https://archive.ics.uci.edu/dataset/241/one+hundred+plant+species+leaves+data+set)

---

## 🧠 Project Objective

* Develop a deep learning-based classification model using CNN architectures.
* Increase accuracy and efficiency over manual leaf identification methods.
* Train and evaluate multiple models to identify the best-performing architecture.

---

## 📦 Dataset Overview

* **Total Samples:** 1600
* **Classes:** 100 plant species
* **Features per Sample:** 64
* **Types of Features:** Shape, Margin, and Texture descriptors
* **Data Format:** `.data` files with label + feature vector

---

## 📊 Models Used

| Model       | Accuracy | Precision | Recall   | F1 Score |
| ----------- | -------- | --------- | -------- | -------- |
| MobileNetV1 | 0.90     | 0.93      | 0.90     | 0.90     |
| MobileNetV2 | **0.91** | **0.95**  | **0.91** | **0.91** |
| InceptionV3 | 0.85     | 0.88      | 0.85     | 0.84     |
| ResNet50    | 0.65     | 0.71      | 0.65     | 0.65     |

> 📌 **Best model**: `MobileNetV2` outperformed others in all evaluation metrics.

---

## 🔍 Workflow Overview

1. **Data Preprocessing**

   * Parsed `.data` files into structured datasets.
   * Normalized inputs.
   * Split into training (80%) and validation (20%).

2. **Model Training**

   * Used TensorFlow and Keras.
   * Employed transfer learning with pretrained CNNs.
   * Fine-tuned hyperparameters with **Keras Hyperband**.

3. **Evaluation**

   * Tracked training/validation accuracy and loss.
   * Plotted performance graphs.
   * Compared precision, recall, F1 score across models.

---

## 🔧 Techniques & Tools

* **Libraries:** TensorFlow, Keras, Keras Tuner, Matplotlib, NumPy
* **Models:** MobileNetV1/V2, InceptionV3, ResNet50
* **Techniques:** CNNs, Transfer Learning, Hyperparameter Tuning



## ✅ Key Findings

* **MobileNetV2** provided the best balance of speed and accuracy for species classification.
* Deep learning can identify subtle patterns in leaf morphology invisible to the human eye.
* Transfer learning is effective even on small biological datasets.
* Using shape-based CNN models can aid conservation and botanical research.

---

## 📌 Future Work

* Augment dataset with real-world leaf images and backgrounds.
* Explore temporal patterns using time-series data (e.g., seasonal leaf changes).
* Deploy as a mobile/web-based leaf recognition app.


