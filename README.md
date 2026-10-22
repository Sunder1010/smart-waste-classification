# Smart Waste Classification using Deep Learning

A Deep Learning based image classification project for automatically identifying different types of waste using **Convolutional Neural Networks (CNN)** and **MobileNetV2 Transfer Learning**.

The project was developed using **Google Colab, TensorFlow/Keras and Kaggle**, with the complete notebook maintained on GitHub.

---

## 📌 Project Overview

Waste segregation is an important part of effective waste management. Manually identifying different categories of waste can be time-consuming.

This project uses Computer Vision and Deep Learning to classify waste images into **12 different categories**.

The project implements:

- Image data inspection and preprocessing
- A custom CNN model as a baseline
- MobileNetV2 based transfer learning
- Model training and evaluation
- Confusion matrix analysis
- Precision, Recall and F1-score evaluation
- Prediction on new unseen images

---

## 🧠 Technologies Used

- Python
- TensorFlow
- Keras
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn
- Google Colab
- Kaggle Dataset
- GitHub

---

## 🗂️ Waste Categories

The model classifies images into the following 12 categories:

1. Battery
2. Biological
3. Brown Glass
4. Cardboard
5. Clothes
6. Green Glass
7. Metal
8. Paper
9. Plastic
10. Shoes
11. Trash
12. White Glass

---

## 🏗️ Project Architecture

### Custom CNN

The baseline CNN consists of:

```text
Input Image
     ↓
Convolutional Layer
     ↓
Max Pooling
     ↓
Convolutional Layer
     ↓
Max Pooling
     ↓
Convolutional Layer
     ↓
Max Pooling
     ↓
Flatten
     ↓
Dense Layer
     ↓
Dropout
     ↓
Output Layer
```

The CNN learns visual features such as edges, textures, shapes and patterns directly from the training images.

---

## 🚀 MobileNetV2 Transfer Learning

The project also uses **MobileNetV2**, a lightweight convolutional neural network architecture designed for efficient image classification.

Instead of learning all visual features from the beginning, transfer learning allows the model to reuse useful features learned from a large image dataset.

The general pipeline is:

```text
Input Waste Image
       ↓
Image Preprocessing
       ↓
MobileNetV2
       ↓
Feature Extraction
       ↓
Classification Layers
       ↓
12 Waste Categories
```

MobileNetV2 was selected because it provides a good balance between classification performance and computational efficiency.

---

## 📊 Model Performance

The final MobileNetV2 model achieved:

| Metric | Result |
|---|---:|
| Test Accuracy | **94.72%** |
| Macro Precision | **0.92** |
| Macro Recall | **0.92** |
| Macro F1-Score | **0.92** |
| Weighted F1-Score | **0.95** |
| Test Images | **2,328** |

The results show that the model generalizes well to unseen test images.

### Strongest Classes

Some of the strongest classification results were:

| Class | Precision | Recall | F1-Score |
|---|---:|---:|---:|
| Clothes | 0.99 | 0.99 | 0.99 |
| Shoes | 0.96 | 0.98 | 0.97 |
| Trash | 0.95 | 0.97 | 0.96 |
| Biological | 0.95 | 0.95 | 0.95 |

### More Challenging Classes

Some visually similar categories were more difficult:

| Class | Precision | Recall | F1-Score |
|---|---:|---:|---:|
| Metal | 0.85 | 0.86 | 0.86 |
| Plastic | 0.91 | 0.82 | 0.86 |
| White Glass | 0.86 | 0.87 | 0.87 |
| Brown Glass | 0.89 | 0.88 | 0.88 |

These differences show why accuracy alone is not enough for evaluating a multi-class classification model.

---

## 🔍 Example Prediction

The trained model was also tested on a new image that was not part of the training process.

Example:

```text
Predicted Class: white-glass
Confidence: 99.59%
```

The prediction pipeline is:

```text
New Image
   ↓
Resize to 224 × 224
   ↓
Normalize Pixel Values
   ↓
MobileNetV2
   ↓
Class Probabilities
   ↓
Highest Probability
   ↓
Predicted Waste Category
```

---

## 📈 Evaluation

The model was evaluated using:

### Accuracy

Measures the percentage of correctly classified images.

### Precision

Measures how many images predicted as a particular class actually belong to that class.

### Recall

Measures how many actual images of a class were correctly identified.

### F1-Score

Provides a balance between precision and recall.

### Confusion Matrix

Used to analyze which waste categories are correctly classified and which categories are confused with each other.

---

## 📁 Repository Structure

```text
smart-waste-classification/
│
├── README.md
│
└── Smart_Waste_Classification.ipynb
```

The complete implementation, experiments, training and evaluation are available in the Jupyter/Colab notebook.

---

## ▶️ How to Run

### 1. Open the notebook

Open:

`Smart_Waste_Classification.ipynb`

using Google Colab.

### 2. Install/Import Dependencies

The notebook contains the required Python libraries.

### 3. Dataset

The project uses a waste image dataset containing the 12 classification categories.

### 4. Run the Notebook

Execute the notebook cells sequentially:

```text
Environment Setup
      ↓
Dataset Setup
      ↓
Data Inspection
      ↓
Preprocessing
      ↓
CNN Baseline
      ↓
MobileNetV2
      ↓
Training
      ↓
Evaluation
      ↓
Confusion Matrix
      ↓
Classification Report
      ↓
New Image Prediction
```

---

## 🎯 Learning Objectives

Through this project, the following Deep Learning concepts were implemented:

- Computer Vision
- Image Classification
- Convolutional Neural Networks
- Convolution and Pooling
- Feature Extraction
- Transfer Learning
- MobileNetV2
- Model Training
- Model Evaluation
- Overfitting Control using Dropout
- Confusion Matrix
- Precision
- Recall
- F1-Score
- Real-world Image Prediction

---

## 🔮 Future Improvements

Possible future improvements include:

- Data augmentation
- Hyperparameter optimization
- Additional waste categories
- Better handling of visually similar classes
- Deployment as a web application
- Real-time camera-based waste classification
- Mobile/edge deployment using TensorFlow Lite

---

## 👨‍💻 Author

**Sunder1010**

GitHub: `Sunder1010`

---

## ⭐ Project Result

The final MobileNetV2 model achieved **94.72% test accuracy** across 12 waste categories, demonstrating that transfer learning can provide strong performance for waste image classification while reducing the amount of training required from scratch.
