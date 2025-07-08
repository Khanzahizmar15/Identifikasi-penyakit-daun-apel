🍏 Apple Leaf Disease Detection using Convolutional Neural Network (CNN)
Final Project — Computer Vision
Name: Nurul Hizmar Khanza
NIM: 2155301111
Class: 4 TI A
Department of Informatics Engineering, Politeknik Caltex Riau
Year: 2025

📌 Background
Apple crops are vulnerable to several diseases, with Powdery Mildew and Rust being among the most common. These diseases can significantly affect the health and yield of apple trees if not detected early.

This project aims to utilize Computer Vision technology and Deep Learning, specifically Convolutional Neural Networks (CNNs), to automatically classify apple leaf images into the following categories:

🟢 Healthy

⚪ Powdery Mildew

🔴 Rust

By providing a fast and reliable detection system, this project supports early diagnosis, allowing for timely intervention and disease control.

🎯 Project Objectives
To develop an image classification model for detecting diseases on apple leaves.

To apply CNN-based deep learning methods for classifying leaf images into three categories: Healthy, Powdery, and Rust.

To provide a practical and usable system using a structured apple leaf image dataset.

🌱 Benefits
✅ For Farmers
Helps farmers quickly identify diseased plants, enabling faster treatment or prevention efforts.

✅ For Agriculture
Promotes healthier crop management using technology, potentially increasing yield and product quality.

🗂️ Dataset
The dataset used in this project is publicly available on Kaggle:
🔗 Plant Disease Recognition Dataset

🧠 Model Architecture & Code Explanation
🔧 Step-by-Step Workflow:
Compile and Train the Model
![image](https://github.com/user-attachments/assets/200e948a-18e4-4dc5-9591-1d9503413c5c)

📈 Model Output & Mobile Integration
✅ Final Accuracy
Training Accuracy: ~94%
Validation Accuracy: ~92%

📉 Accuracy Graph (Training vs Validation)
Example graph to be added in the repo: accuracy_plot.png
Shows convergence of training and validation accuracy across 25 epochs.

📲 Mobile Deployment
The trained model was successfully converted to .tflite format and integrated into an Android app using Android Studio.

MainActivity.kt: Handles image selection and invokes the model for prediction.
![image](https://github.com/user-attachments/assets/74018677-b091-41d1-99eb-769ccbc678d1)

MainActivity.xml: UI for loading an image and displaying the prediction result.
![image](https://github.com/user-attachments/assets/88b1c0fb-28ac-4ffb-88b5-f21b03027ca1)

📸 Mobile UI Example
![image](https://github.com/user-attachments/assets/4ef9ec6b-820c-4707-9089-17d8e9c12d35)
![image](https://github.com/user-attachments/assets/b4d5a275-6601-49d2-8eb1-7d937a651a16)
![image](https://github.com/user-attachments/assets/15243b01-8737-4e3d-9011-fd46397e6af3)
![image](https://github.com/user-attachments/assets/c49d6bb7-555e-4235-ade7-d12d0f7de1ca)

🔍 Challenges & Observations
Image Quality Test
20 blurry or noisy images were added to the training set to test model robustness.

✅ Result: The model was still able to achieve good performance with ~94% training accuracy and ~92% validation accuracy.

Generalization Ability
Despite noisy inputs, the model demonstrated resilience, suggesting effective generalization on slightly imperfect images.

✅ Conclusion
This project developed an effective system for detecting apple leaf diseases using Convolutional Neural Networks (CNN). It shows promising performance and potential for real-world use by farmers and agricultural stakeholders. Integration with mobile platforms further increases accessibility, making this a practical tool for smart farming.

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
