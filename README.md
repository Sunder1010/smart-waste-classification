# ♻️ Smart Waste Classification using Deep Learning

A Deep Learning and Computer Vision project that classifies waste images into **12 different waste categories** using a custom CNN and **MobileNetV2 Transfer Learning**.

The project demonstrates an end-to-end image classification workflow including dataset preparation, image preprocessing, CNN model development, transfer learning, model training, evaluation, visualization, and real-world image prediction.

---

## 🎯 Project Objective

The objective of this project is to build an automated waste classification system that can identify the type of waste from an input image.

Accurate waste classification can support better waste segregation and recycling by helping identify materials such as plastic, paper, metal, glass, cardboard, and biological waste.

---

## 🧠 Deep Learning Approach

Two approaches were implemented and compared:

### 1. Custom CNN

A Convolutional Neural Network was developed from scratch using:

- Convolutional layers
- Max Pooling
- Flatten
- Dense layers
- Dropout
- Softmax classification

### 2. MobileNetV2 Transfer Learning

A pretrained **MobileNetV2** model was used as the main transfer-learning approach.

MobileNetV2 was selected because it provides strong image feature extraction while remaining relatively lightweight and efficient compared with larger CNN architectures.

---

## 🔄 Project Workflow

```text
Waste Image
     ↓
Dataset Preparation
     ↓
Image Resizing (224 × 224)
     ↓
Image Normalization
     ↓
Data Augmentation
     ↓
     ┌──────────────────────┐
     │                      │
     ↓                      ↓
Custom CNN            MobileNetV2
     │                Transfer Learning
     ↓                      ↓
Feature Learning     Feature Extraction
     │                      │
     └──────────┬───────────┘
                ↓
        Classification
                ↓
       12 Waste Classes
                ↓
      Prediction + Confidence
```

---

## 🗂️ Waste Categories

The model classifies images into 12 categories:

- Battery
- Biological
- Brown Glass
- Cardboard
- Clothes
- Green Glass
- Metal
- Paper
- Plastic
- Shoes
- Trash
- White Glass

---

## 🛠️ Technologies Used

| Technology | Purpose |
|---|---|
| Python | Programming language |
| TensorFlow | Deep Learning framework |
| Keras | Neural network API |
| MobileNetV2 | Transfer learning model |
| NumPy | Numerical operations |
| Matplotlib | Data visualization |
| Seaborn | Confusion matrix visualization |
| Scikit-learn | Model evaluation |
| Google Colab | Model development and training |
| Kaggle | Dataset source |
| GitHub | Version control and project documentation |

---

## 📊 Model Performance

The final MobileNetV2 model achieved:

**Test Accuracy: ~94.72%**

The classification report also achieved approximately:

- Weighted Precision: **0.95**
- Weighted Recall: **0.95**
- Weighted F1-Score: **0.95**

The model was evaluated on **2,328 test images**.

---

## 📈 Evaluation Results

The repository contains visualizations of the model performance:

### Training Accuracy

Shows the training and validation accuracy across epochs.

### Training Loss

Shows how training and validation loss changed during model training.

### Confusion Matrix

Shows the number of correct and incorrect predictions for each waste category.

### Model Comparison

Compares the validation performance of the custom CNN and MobileNetV2 models.

---

## 🔬 Example Prediction

The trained MobileNetV2 model was also tested on a previously unseen image.

Example:

```text
Predicted Class: White Glass
Confidence: 99.59%
```

This demonstrates how the trained model can be used for individual image inference.

---

## 🧪 Model Evaluation Metrics

The project uses several standard classification metrics:

### Accuracy

Measures the percentage of correctly classified images.

### Precision

Measures how many images predicted as a particular class actually belong to that class.

### Recall

Measures how many actual samples of a class were correctly identified.

### F1-Score

Combines precision and recall into a single metric.

### Confusion Matrix

Provides a class-by-class view of correct and incorrect predictions.

---

## 📁 Repository Structure

```text
smart-waste-classification/
│
├── Smart_Waste_Classification.ipynb
├── README.md
├── requirements.txt
│
└── results/
    ├── confusion_matrix (1).png
    ├── model_comparison (1).png
    ├── training_accuracy (1).png
    └── training_loss (1).png
```

---

## 🚀 How to Run

### 1. Clone the repository

```bash
git clone https://github.com/Sunder1010/smart-waste-classification.git
```

### 2. Open the notebook

Open:

```text
Smart_Waste_Classification.ipynb
```

The notebook can be executed using Google Colab.

### 3. Install dependencies

```bash
pip install -r requirements.txt
```

### 4. Run the notebook

The notebook contains the complete workflow:

```text
Dataset
→ Preprocessing
→ Model Building
→ Training
→ Evaluation
→ Prediction
```

---

## 💡 Key Learning Outcomes

Through this project, I worked with:

- Convolutional Neural Networks
- Transfer Learning
- MobileNetV2
- Image preprocessing
- Data augmentation
- Model training and validation
- Overfitting prevention using Dropout
- Classification reports
- Confusion matrices
- Model comparison
- Single-image inference
- TensorFlow/Keras
- Google Colab
- Kaggle datasets
- GitHub project management

---

## 🔮 Future Improvements

Possible future improvements include:

- Building a web application for real-time prediction
- Deploying the model using Streamlit
- Optimizing the model for mobile/edge devices
- Adding more waste categories
- Increasing dataset diversity
- Improving performance on visually similar classes
- Adding explainable AI techniques such as Grad-CAM
- Real-time camera-based waste classification

---

## 👨‍💻 Author

**Sunder1010**

Master of Computer Applications (MCA)

GitHub:  
https://github.com/Sunder1010

---

## ⭐ Project Highlights

**94.72% Test Accuracy | MobileNetV2 Transfer Learning | 12-Class Waste Classification | TensorFlow/Keras | Computer Vision**
