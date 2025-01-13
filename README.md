# Brain Tumor Detector

![Deep Learning](https://img.shields.io/badge/Deep%20Learning-TensorFlow-orange?style=for-the-badge)
![Flask](https://img.shields.io/badge/Backend-Flask-blue?style=for-the-badge)
![Bootstrap](https://img.shields.io/badge/Frontend-Bootstrap-purple?style=for-the-badge)
![Python](https://img.shields.io/badge/Language-Python-brightgreen?style=for-the-badge)
![Pillow](https://img.shields.io/badge/Image%20Processing-Pillow-yellow?style=for-the-badge)
![Matplotlib](https://img.shields.io/badge/Visualization-Matplotlib-blue?style=for-the-badge)
![Seaborn](https://img.shields.io/badge/Visualization-Seaborn-green?style=for-the-badge)
![NumPy](https://img.shields.io/badge/Numerical%20Computing-NumPy-orange?style=for-the-badge)
![License](https://img.shields.io/badge/License-MIT-lightgrey?style=for-the-badge)

## Project Overview

The **Brain Tumor Detector** is a deep learning-powered web application designed to classify brain tumors based on MRI scans. This project integrates advanced computer vision techniques with a user-friendly web interface, enabling users to upload MRI images and obtain predictions about the presence and type of brain tumor with confidence scores. The application supports the classification of four categories:

- **Pituitary Tumor**
- **Glioma Tumor**
- **Meningioma Tumor**
- **No Tumor**

This project aims to demonstrate the potential of AI in medical diagnostics by automating the analysis of medical imaging data.

---

## Features

- **Tumor Classification**: Identifies if the MRI scan contains a tumor and its type.
- **Confidence Scores**: Displays the model's confidence in its prediction.
- **User-Friendly Interface**: Simple and intuitive web interface for uploading MRI images and displaying results.
- **Fast Inference**: Utilizes a pre-trained deep learning model for efficient and accurate predictions.
- **Data Visualization**: Includes plots and insights generated using Matplotlib and Seaborn.

---

## Tech Stack

### **Frontend**
![HTML](https://img.shields.io/badge/HTML-E34F26?style=for-the-badge&logo=html5&logoColor=white)
![CSS](https://img.shields.io/badge/CSS-1572B6?style=for-the-badge&logo=css3&logoColor=white)
![Bootstrap](https://img.shields.io/badge/Bootstrap-7952B3?style=for-the-badge&logo=bootstrap&logoColor=white)

### **Backend**
![Flask](https://img.shields.io/badge/Flask-000000?style=for-the-badge&logo=flask&logoColor=white)

### **Deep Learning**
![TensorFlow](https://img.shields.io/badge/TensorFlow-FF6F00?style=for-the-badge&logo=tensorflow&logoColor=white)
![Keras](https://img.shields.io/badge/Keras-D00000?style=for-the-badge&logo=keras&logoColor=white)

### **Programming Language**
![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)

### **Image Processing**
![Pillow](https://img.shields.io/badge/Pillow-3776AB?style=for-the-badge&logo=python&logoColor=white)

### **Data Visualization**
![Matplotlib](https://img.shields.io/badge/Matplotlib-3776AB?style=for-the-badge&logo=python&logoColor=white)
![Seaborn](https://img.shields.io/badge/Seaborn-3776AB?style=for-the-badge&logo=python&logoColor=white)

### **Numerical Computing**
![NumPy](https://img.shields.io/badge/NumPy-013243?style=for-the-badge&logo=numpy&logoColor=white)

---

## Dataset

The model is trained on the **Brain Tumor Dataset**, a publicly available dataset that contains labeled MRI scans. The dataset includes the following categories:

- **Pituitary Tumor**
- **Glioma Tumor**
- **Meningioma Tumor**
- **No Tumor**

Preprocessing steps include resizing images to 128x128 pixels, normalization, and data augmentation to improve model generalization.

---

## Model Architecture

The deep learning model is based on **VGG16**, a pre-trained convolutional neural network (CNN). Key highlights:

- **Pre-trained Weights**: Uses ImageNet weights for transfer learning.
- **Fine-tuning**: Freezes earlier layers and fine-tunes the last few layers for the brain tumor dataset.
- **Regularization**: Includes dropout layers to prevent overfitting.

### Model Summary

1. Input Layer: Image size (128x128x3)
2. Base Model: VGG16 (with frozen layers)
3. Flatten Layer
4. Dense Layers with ReLU activation
5. Dropout Layers for regularization
6. Output Layer: Softmax activation for multi-class classification

---

## Installation

Follow these steps to run the project locally:

### Prerequisites
- Python 3.8 or higher
- Virtual environment setup (recommended)

### Steps
1. Clone the repository:
   ```bash
   git clone https://github.com/Shikhararora19/BrainTumorDetector.git
   cd BrainTumorDetector
   ```

2. Create and activate a virtual environment:
   ```bash
   python3 -m venv venv
   source venv/bin/activate  # On Windows: venv\Scripts\activate
   ```

3. Install the dependencies:
   ```bash
   pip install -r requirements.txt
   ```

4. Run the Flask application:
   ```bash
   python main.py
   ```

5. Open your browser and navigate to:
   ```
   http://127.0.0.1:5000
   ```

---

## Usage

1. Upload an MRI image in `.png`, `.jpg`, or `.jpeg` format.
2. Click the "Predict" button to analyze the image.
3. View the prediction and confidence score on the results page.


---

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

---

## Acknowledgments

- **Dataset**: Brain Tumor Dataset (Publicly available on kaggle).
- **Frameworks**: TensorFlow, Keras, Flask, and Bootstrap.
- **Libraries**: Matplotlib, Seaborn, NumPy, and Pillow.

---

### Author

- **Shikhar Arora**
- GitHub: [Shikhararora19](https://github.com/Shikhararora19)
