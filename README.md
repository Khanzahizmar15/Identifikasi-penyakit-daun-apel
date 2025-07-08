🍏 Apple Leaf Disease Detection using Convolutional Neural Network (CNN)
🎓 Final Project — Computer Vision
Name: Nurul Hizmar Khanza
NIM: 2155301111
Class: 4 TI A
Department: Informatics Engineering
Institution: Politeknik Caltex Riau
Year: 2025

📌 Background
Apple crops are susceptible to various plant diseases, with Powdery Mildew and Rust being among the most prevalent. These conditions can severely impact the health and yield of apple trees if not detected early.

This project leverages Computer Vision and Deep Learning, specifically Convolutional Neural Networks (CNNs), to classify apple leaf images into the following categories:

🟢 Healthy

⚪ Powdery Mildew

🔴 Rust

By offering a fast and accurate detection system, this project supports early diagnosis and timely intervention, enhancing disease management and crop protection.

🎯 Project Objectives
Develop a CNN-based image classification model to detect diseases on apple leaves.

Classify apple leaf images into three classes: Healthy, Powdery Mildew, and Rust.

Provide a reliable and deployable solution using a structured leaf image dataset.

🌱 Benefits
✅ For Farmers
Enables early detection of leaf diseases, allowing quicker responses to prevent spread and damage.

✅ For Agriculture Sector
Supports smart farming practices, improves crop management, and contributes to better agricultural productivity.

🗂️ Dataset
The dataset used in this project is publicly available on Kaggle:
🔗 Plant Disease Recognition Dataset

🧠 Model Architecture & Code Overview
🔧 Step-by-Step Implementation
Mount Google Drive

To load the dataset and save the trained model.

Count Dataset Images

Ensures image distribution is correct across train, test, and validation sets.

Visualize Sample Images

Displays random leaf images to verify data quality.

Preprocessing with ImageDataGenerator

Augmentation: Random rotation, zoom, flipping to increase diversity.

Rescaling: Normalize pixel values to [0, 1].

Create Data Generators

Loads images in batches directly from folders for training and validation.

Build CNN Architecture

Layers used:

Conv2D (feature extraction)

MaxPooling2D (dimensionality reduction)

Flatten (convert 2D to 1D)

Dense (fully connected layers with softmax for multi-class output)

Compile the Model

Loss: categorical_crossentropy

Optimizer: adam

Metric: accuracy

Train the Model

Trained for 25 epochs using training and validation sets.

Show Final Accuracy

Printed final training and validation accuracy after training completes.

Visualize Accuracy Graph

Accuracy vs. Epochs chart helps monitor learning progress and detect overfitting.

Save Model

Stored in .h5 format for reuse or deployment.

Predict New Image

Preprocess external image and predict class using the trained model.

Decode Prediction

Maps predicted class index to human-readable labels.

Convert to TensorFlow Lite

Converts model to .tflite for mobile use.

📈 Model Output & Mobile Integration
✅ Final Accuracy
Training Accuracy: ~94%

Validation Accuracy: ~92%

📉 Accuracy Graph
Displays training and validation accuracy over 25 epochs:
📍 (Sample graph accuracy_plot.png can be added to your repo)

📲 Mobile Deployment
The trained model was successfully converted into TensorFlow Lite format and integrated into an Android application using Android Studio (Kotlin).

🔹 MainActivity.kt
Handles image loading, preprocessing, and prediction.



🔹 MainActivity.xml
Provides a simple interface to upload a leaf image and display the prediction.



📸 Mobile App UI Examples
<div align="center"> <img src="https://github.com/user-attachments/assets/4ef9ec6b-820c-4707-9089-17d8e9c12d35" width="200"/> <img src="https://github.com/user-attachments/assets/b4d5a275-6601-49d2-8eb1-7d937a651a16" width="200"/> <img src="https://github.com/user-attachments/assets/15243b01-8737-4e3d-9011-fd46397e6af3" width="200"/> <img src="https://github.com/user-attachments/assets/c49d6bb7-555e-4235-ade7-d12d0f7de1ca" width="200"/> </div>
🔍 Challenges & Observations
🧪 Image Quality Test
Introduced 20 blurry or noisy apple leaf images into the training set.

✅ Result:
The model remained robust and achieved high accuracy (~94% training, ~92% validation), showing good generalization.

✅ Conclusion
This project demonstrates the successful application of Convolutional Neural Networks (CNNs) for classifying apple leaf diseases. The system is accurate, efficient, and adaptable for mobile deployment via TensorFlow Lite and Android Studio — making it a practical solution for real-time field use by farmers.

🚀 Technologies Used
Python 🐍

TensorFlow / Keras

Convolutional Neural Network (CNN)

NumPy, Pandas, Matplotlib

Google Colab

TensorFlow Lite

Android Studio (Kotlin)

Made with ❤️ by Nurul Hizmar Khanza
Politeknik Caltex Riau — 2025

