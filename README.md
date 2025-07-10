# 🩺 Breast Cancer Detection Using Deep Learning

This project implements a deep learning-based solution for classifying mammogram images as **Benign** or **Malignant** using a fine-tuned ResNet50 model. Built with TensorFlow and Keras, the model applies transfer learning to enhance the early detection of breast cancer through image-based diagnosis.

---

## 🧠 Project Overview

Breast cancer is one of the leading causes of mortality among women globally. Early detection is critical for effective treatment. This project explores the application of computer vision and transfer learning to support breast cancer diagnosis from mammographic images.

Using a pre-trained ResNet50 model as the feature extractor, the system is fine-tuned with custom classification layers to distinguish between benign and malignant cases. The model accepts user-uploaded images and predicts the likelihood of cancer in real-time.

---

## 📁 Dataset (Demo Version)

- The current version of this project is trained using **synthetic demo data** (randomly generated images and labels) to demonstrate model integration, training, and prediction workflow.
- Real-world testing has been performed using publicly available mammogram images.
- Future enhancements will include integration with clinical datasets (e.g., DDSM, CBIS-DDSM, or BreakHis).

---

## 🧰 Technologies Used

- **Language**: Python  
- **Frameworks**: TensorFlow, Keras  
- **Model Architecture**: ResNet50 (Transfer Learning)  
- **Development Environment**: Google Colab  
- **Libraries**: NumPy, Matplotlib, PIL

---

## 🏗️ Model Architecture

- **Base Model**: ResNet50 (pre-trained on ImageNet, `include_top=False`)
- **Added Layers**:
  - `GlobalAveragePooling2D`
  - `Dense(1024, activation='relu')`
  - `Dense(2, activation='softmax')`
- **Loss Function**: Categorical Crossentropy  
- **Optimizer**: Adam (learning rate = 0.001)  
- **Metrics**: Accuracy

---

## 🚀 How to Use

1. **Clone the Repository**
   ```bash
   git clone https://github.com/Vinuthnadivi/Breast_Cancer_Detection.git
   cd Breast_Cancer_Detection
