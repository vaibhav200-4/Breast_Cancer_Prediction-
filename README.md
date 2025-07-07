# 🩺 Breast Cancer Prediction using Artificial Neural Network (ANN)

This project aims to predict whether a breast tumor is **benign** or **malignant** using an Artificial Neural Network (ANN) model trained on the **Breast Cancer Wisconsin Diagnostic dataset**.

---

## 📊 Dataset Information

The dataset contains features computed from a digitized image of a breast mass's fine needle aspirate (FNA). It includes measurements describing the characteristics of the cell nuclei present in the image.

- 📦 **Total Samples:** 569  
- 📊 **Features:** 30 numeric attributes  
- 🎯 **Target:** `diagnosis` (M = Malignant, B = Benign)

---

## 📁 Features Overview

- `radius_mean`, `texture_mean`, `perimeter_mean`, `area_mean`, `smoothness_mean`, ...
- Standard errors: `radius_se`, `texture_se`, ...
- Worst values: `radius_worst`, `texture_worst`, ...

👉 Features represent the mean, standard error, and worst values for different measurements of each tumor.

---

## 🚀 Project Workflow

1. **Data Cleaning**
   - Removed `id` and empty `Unnamed: 32` columns
   - Encoded `diagnosis` (M=1, B=0)

2. **Data Scaling**
   - Standardized feature values using `StandardScaler` for better ANN performance

3. **Model Building**
   - Created an ANN model using TensorFlow Keras
   - 2 hidden layers with ReLU activation
   - Output layer with Sigmoid activation (for binary classification)

4. **Model Training**
   - Trained on 80% of data with 20% reserved for testing
   - Used `binary_crossentropy` as loss and `Adam` optimizer

5. **Model Evaluation**
   - Evaluated accuracy on test data

---

## 📈 Model Architecture

- **Input Layer:** 30 neurons  
- **Hidden Layer 1:** 16 neurons (ReLU)  
- **Hidden Layer 2:** 8 neurons (ReLU)  
- **Output Layer:** 1 neuron (Sigmoid)  

---

## 📊 Results

- Achieved **~96% accuracy** on training data
- Achieved **~95% accuracy** on test data

---

## 📦 Libraries Used

- `pandas`
- `numpy`
- `matplotlib`
- `seaborn`
- `scikit-learn`
- `tensorflow` / `keras`

---

## 📌 How to Run

1. Clone the repository  
