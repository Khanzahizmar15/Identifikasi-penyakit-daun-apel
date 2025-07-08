# 🍏 Apple Leaf Disease Detection using Convolutional Neural Network (CNN)

🎓 **Final Project — Computer Vision**  
**Name:** Nurul Hizmar Khanza  
**NIM:** 2155301111  
**Class:** 4 TI A  
**Department:** Informatics Engineering  
**Institution:** Politeknik Caltex Riau  
**Year:** 2025  

---

## 📌 Background

Apple crops are susceptible to various plant diseases, with **Powdery Mildew** and **Rust** being among the most prevalent. These conditions can severely impact the health and yield of apple trees if not detected early.

This project leverages **Computer Vision** and **Deep Learning**, specifically **Convolutional Neural Networks (CNNs)**, to classify apple leaf images into the following categories:

- 🟢 **Healthy**
- ⚪ **Powdery Mildew**
- 🔴 **Rust**

By offering a fast and accurate detection system, this project supports early diagnosis and timely intervention, enhancing disease management and crop protection.

---

## 🎯 Project Objectives

- Develop a CNN-based image classification model to detect diseases on apple leaves.
- Classify apple leaf images into three classes: **Healthy**, **Powdery Mildew**, and **Rust**.
- Provide a reliable and deployable solution using a structured leaf image dataset.

---

## 🌱 Benefits

### ✅ For Farmers
- Enables early detection of leaf diseases, allowing quicker responses to prevent spread and damage.

### ✅ For Agriculture Sector
- Supports smart farming practices.
- Improves crop management.
- Contributes to better agricultural productivity.

---

## 🗂️ Dataset

The dataset used in this project is publicly available on Kaggle:  
🔗 [Plant Disease Recognition Dataset](https://www.kaggle.com/datasets/emmarex/plantdisease)

---

## 🧠 Model Architecture & Code Overview

### 🔧 Step-by-Step Implementation

1. **Mount Google Drive**  
   - Load dataset and save trained model.

2. **Count Dataset Images**  
   - Ensure proper image distribution across training, validation, and test sets.

3. **Visualize Sample Images**  
   - Display random leaf images to verify data quality.

4. **Preprocessing with `ImageDataGenerator`**  
   - **Augmentation:** Random rotation, zoom, and flipping.  
   - **Rescaling:** Normalize pixel values to `[0, 1]`.

5. **Create Data Generators**  
   - Load images in batches for training and validation.

6. **Build CNN Architecture**  
   - `Conv2D`, `MaxPooling2D`, `Flatten`, `Dense` with `softmax`.

7. **Compile the Model**  
   - **Loss:** `categorical_crossentropy`  
   - **Optimizer:** `adam`  
   - **Metric:** `accuracy`

8. **Train the Model**  
   - Train for 25 epochs.

9. **Show Final Accuracy**  
   - Display training and validation accuracy.

10. **Visualize Accuracy Graph**  
    - Plot accuracy vs. epochs to monitor overfitting.

11. **Save Model**  
    - Save as `.h5` file.

12. **Predict New Image**  
    - Preprocess external image and predict class.

13. **Decode Prediction**  
    - Convert class index to readable label.

14. **Convert to TensorFlow Lite**  
    - Convert model to `.tflite` for mobile deployment.

---

## 📈 Model Output & Mobile Integration

### ✅ Final Accuracy
- **Training Accuracy:** ~94%  
- **Validation Accuracy:** ~92%

### 📉 Accuracy Graph
Displays training and validation accuracy over 25 epochs.  
📍 *(You can add `accuracy_plot.png` to your repository for reference)*

### 📲 Mobile Deployment
The trained model was successfully converted into **TensorFlow Lite** format and integrated into an Android application using **Android Studio (Kotlin)**.

- `MainActivity.kt`: Handles image loading, preprocessing, and prediction.
- `MainActivity.xml`: Provides UI to upload a leaf image and display prediction.

### 📸 Mobile App UI Examples

<div align="center">
  <img src="https://github.com/user-attachments/assets/4ef9ec6b-820c-4707-9089-17d8e9c12d35" width="200"/>
  <img src="https://github.com/user-attachments/assets/b4d5a275-6601-49d2-8eb1-7d937a651a16" width="200"/>
  <img src="https://github.com/user-attachments/assets/15243b01-8737-4e3d-9011-fd46397e6af3" width="200"/>
  <img src="https://github.com/user-attachments/assets/c49d6bb7-555e-4235-ade7-d12d0f7de1ca" width="200"/>
</div>

---

## 🔍 Challenges & Observations

### 🧪 Image Quality Test
Tested the model by introducing 20 blurry/noisy apple leaf images into the training set.

### ✅ Result:
- Model remained robust.
- Maintained high accuracy (~94% training, ~92% validation).
- Demonstrated good generalization.

---

## ✅ Conclusion

This project demonstrates the successful application of **CNNs** for classifying apple leaf diseases. The system is:

- ✅ Accurate  
- ✅ Efficient  
- ✅ Mobile-friendly via TensorFlow Lite  
- ✅ Practical for real-time field use by farmers

---

## 🚀 Technologies Used

- Python 🐍  
- TensorFlow / Keras  
- CNN (Convolutional Neural Networks)  
- NumPy, Pandas, Matplotlib  
- Google Colab  
- TensorFlow Lite  
- Android Studio (Kotlin)  

---

**Made with ❤️ by Nurul Hizmar Khanza**  
*Politeknik Caltex Riau — 2025*
