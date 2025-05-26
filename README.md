# 🎵 Musical Instrument Classificator  
### *by Juan David Velásquez R.*

Welcome to the **Musical Instrument Classificator**, an intelligent solution built to automate the classification of musical instruments for an online store. This project was developed to streamline inventory and category management for e-commerce owners, saving time and ensuring consistent organization across the platform.

---

## 🧠 Project Overview

This intelligent system leverages an **ensemble learning strategy** to classify musical instrument images with high accuracy. It was designed to significantly reduce the manual effort required to organize and manage product listings in an online store.

---

## 🛠️ Technologies Used

This project combines deep learning and gradient boosting to achieve robust, high-performing results.

### 🔹 Base Models:
- `EfficientNet-B1`
- `EfficientNet-B2`
- `EfficientNet-B3`

These convolutional neural networks (CNNs) serve as visual feature extractors and make initial predictions based on instrument images.

### 🔹 Meta Model:
- `CatBoostClassifier`  
This powerful gradient boosting model receives the outputs of the base models and learns how to combine them optimally, increasing overall classification accuracy.

---

## 🔁 Ensemble Strategy

The architecture follows a **stacking ensemble approach**:

1. The EfficientNet models individually process input images and generate predictions.
2. These predictions are used as features for the CatBoost meta model.
3. CatBoost learns from the base model outputs and refines the final classification decision.

This layered strategy allows the system to harness the strengths of each model and improve predictive performance.

---

## 🎯 Key Benefits

- ✅ Automates manual classification, saving time and effort
- ✅ Increases accuracy through ensemble learning
- ✅ Ensures consistent product categorization
- ✅ Easily scalable to include more instruments or categories

---

## ⚙️ Requirements

To run this project, you’ll need:

- Python 3.8+
- TensorFlow / Keras
- CatBoost
- NumPy, Pandas, Scikit-learn
- Matplotlib or Seaborn (for visualization)
