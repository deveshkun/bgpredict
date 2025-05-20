# 🧬 Fingerprint-Based Blood Group Classification

A final year B.Tech project that uses a **hybrid approach combining CNN and handcrafted features** to classify blood groups (A, B, AB, O with Rh+/-) based on fingerprint images.

---

## 📌 Project Overview

This project explores a novel method for **blood group prediction from fingerprint images** using a blend of **deep learning** and **feature engineering**. It aims to improve classification performance by combining convolutional features extracted via CNN with handcrafted features such as:

- Ridge endings
- Bifurcations
- Ridge/valley thickness
- Ridge frequency
- Local Binary Pattern (LBP)
- Orientation features
- Wavelet features

The combined feature vector is used to train a high-performance **Artificial Neural Network (ANN)** classifier.

---

## 🔍 Key Features

- 📷 Custom fingerprint dataset labeled with blood groups
- 🧠 CNN-based convolutional feature extraction
- 🧪 Manual feature extraction (LBP, wavelet, ridge/valley, etc.)
- ⚖️ SMOTE for class balancing
- 🔍 PCA for dimensionality reduction
- 📈 Final ANN model trained on combined features
- 🧾 Features exported to CSV for reproducibility
- 🌐 Flask-based web app for prediction (optional)

---

## 🛠️ Tech Stack

- Python 3.x
- TensorFlow / Keras
- OpenCV, NumPy, Pandas
- scikit-learn
- imbalanced-learn (SMOTE)
- PyWavelets
- Flask (for deployment)

---

## 🗂️ Folder Structure
Fingerprint-BloodGroup-Classification/
│
├── dataset_blood_group/ # Fingerprint images categorized by blood group
├── features/ # Extracted handcrafted + CNN features
├── models/ # Saved models (final_model.h5, CNN model, etc.)
├── csv_outputs/ # Combined feature vectors as CSV
├── flask_app/ # Flask web app for prediction
├── utils/ # Helper scripts for feature extraction, preprocessing
├── notebooks/ # Jupyter notebooks for EDA & experiments
├── main_training_script.py # Final training pipeline
└── README.md # Project overview and usage

