# 🧠 Brain Tumor Detection using CNN

A deep learning project for detecting brain tumors from MRI scans using a **Convolutional Neural Network (CNN)** built with TensorFlow/Keras. The system classifies MRI images as **Tumour** or **No Tumour** and additionally highlights the suspected tumour region using an OpenCV-based localization technique.

---

## 📌 Project Overview

Brain tumor diagnosis from MRI scans is a critical medical imaging task. This project demonstrates how deep learning can be applied to automate tumour detection using a CNN trained on MRI images.

### Key Capabilities

* ✅ Binary classification of MRI scans
* ✅ Tumour vs No Tumour prediction
* ✅ Automatic tumour localization using red bounding boxes
* ✅ Data augmentation for improved generalization
* ✅ Early stopping to prevent overfitting
* ✅ Model evaluation using confusion matrix and classification metrics

---

## 🗂 Dataset

**Dataset Used:**

Brain MRI Images for Brain Tumor Detection

Kaggle Dataset:
https://www.kaggle.com/datasets/navoneel/brain-mri-images-for-brain-tumor-detection

### Dataset Structure

brain_tumor_dataset/
├── yes/
└── no/

* Tumour Images: 155
* No Tumour Images: 98

---

## 🏗 Model Architecture

The CNN architecture consists of:

* 3 Convolutional Layers
* 3 Max Pooling Layers
* Flatten Layer
* Dense Layer (128 neurons)
* Dropout Layer (0.5)
* Sigmoid Output Layer

### Model Summary

* Total Parameters: **3,304,769**
* Trainable Parameters: **3,304,769**

### Architecture Screenshot

![Model Architecture](https://github.com/arshan-rahman/Brain-Tumor-Detection-CNN/blob/fb20758d98ca967c13caf604a9005dfdda442a80/img1)

---

## ⚙️ Technologies Used

* Python
* TensorFlow / Keras
* OpenCV
* NumPy
* Matplotlib
* Seaborn
* Scikit-learn
* Google Colab

---

## 🔄 Workflow

1. Load MRI dataset
2. Preprocess images
3. Resize images to 128 × 128
4. Normalize pixel values
5. Split into training and testing datasets
6. Apply data augmentation
7. Train CNN model
8. Evaluate model performance
9. Predict new MRI images
10. Highlight suspected tumour regions

---

## 📊 Model Evaluation

### Confusion Matrix

The confusion matrix obtained on the test dataset is shown below.

![Confusion Matrix](https://github.com/arshan-rahman/Brain-Tumor-Detection-CNN/blob/6efa3aed2d68856255bc521f233ce675a417fd8f/Screenshot%202026-06-22%20134951.png)

### Results

| Metric          | Value |
| --------------- | ----- |
| True Negatives  | 13    |
| False Positives | 7     |
| False Negatives | 2     |
| True Positives  | 29    |

The model demonstrates strong tumour detection capability with a low number of missed tumour cases.

---

## 🧪 Tumour Detection Example

When an MRI image is classified as containing a tumour, the system identifies the most suspicious bright region inside the brain and highlights it using a red bounding box.

### Prediction Example

![Tumour Detection](https://github.com/arshan-rahman/Brain-Tumor-Detection-CNN/blob/6efa3aed2d68856255bc521f233ce675a417fd8f/Screenshot%202026-06-22%20135023.png)

Example Prediction:

Prediction: Tumour Detected

Probability: 0.9676

---

## 🚀 How to Run

### Clone the Repository

```bash
git clone https://github.com/YOUR_USERNAME/brain-tumor-detection-cnn.git
cd brain-tumor-detection-cnn
```

### Install Dependencies

```bash
pip install -r requirements.txt
```

### Download Dataset

Download the dataset from Kaggle:

https://www.kaggle.com/datasets/navoneel/brain-mri-images-for-brain-tumor-detection

Extract it into the project directory.

### Run the Notebook

Open and execute:

```bash
brain_tumor_detection.ipynb
```

---

## 🔮 Future Improvements

* Grad-CAM based explainability
* U-Net based tumour segmentation
* Web application deployment using Streamlit
* Improved localization using segmentation masks
* Multi-class brain tumour classification

---

## ⚠️ Disclaimer

This project is intended for educational and research purposes only. It should not be used for clinical diagnosis or medical decision-making.

---

## 👨‍💻 Author

Developed as a deep learning and computer vision project to explore the application of CNNs in medical image analysis.

If you found this project useful, consider giving it a ⭐ on GitHub.
