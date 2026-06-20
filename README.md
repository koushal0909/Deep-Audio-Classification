# 🎧 Deep Audio Classification using Machine Learning & Deep Learning

## 📌 Overview

Deep Audio Classification is a machine learning and deep learning project that classifies environmental sounds into predefined categories using audio signal processing techniques and neural networks.

The project utilizes the **UrbanSound8K dataset**, extracts **Mel-Frequency Cepstral Coefficients (MFCCs)** from audio files, and trains a **Deep Neural Network (DNN)** to recognize and classify sounds such as dog barks, sirens, drilling, street music, and more.

The performance of the DNN is further compared with traditional machine learning models including **Random Forest** and **XGBoost**.

---

## 🎯 Objective

The primary objectives of this project are:

* Build an end-to-end audio classification pipeline.
* Extract meaningful audio features using MFCC.
* Train and evaluate a Deep Neural Network for sound recognition.
* Compare DNN performance with Random Forest and XGBoost models.
* Perform classification on custom audio samples.
* Analyze model performance using visualization and evaluation metrics.

---

## 📂 Dataset

### UrbanSound8K

The project uses the **UrbanSound8K** dataset containing:

* **8,732 labeled audio samples**
* **10 environmental sound classes**
* Approximately **6 GB** in size

### Sound Classes

* Air Conditioner
* Car Horn
* Children Playing
* Dog Bark
* Drilling
* Engine Idling
* Gun Shot
* Jackhammer
* Siren
* Street Music

Dataset Link:

https://urbansounddataset.weebly.com/urbansound8k.html

---

## 🛠️ Technologies Used

### Programming Language

* Python

### Development Environment

* Jupyter Notebook

### Libraries

* NumPy
* Pandas
* Librosa
* Matplotlib
* Seaborn
* Scikit-learn
* TensorFlow
* Keras
* XGBoost
* TQDM

---

## ⚙️ Project Workflow

### 1. Data Loading

* UrbanSound8K metadata is loaded.
* Audio files are accessed using their fold structure.

### 2. Feature Extraction

For each audio file:

* Audio is loaded using Librosa.
* 40 MFCC features are extracted.
* Mean and standard deviation of MFCCs are computed.
* Features are combined into an 80-dimensional feature vector.

### 3. Data Preprocessing

* Label Encoding
* One-Hot Encoding
* Train-Test Split
* Feature Scaling using StandardScaler

### 4. Model Training

A Deep Neural Network (DNN) is built using TensorFlow/Keras.

Architecture:

Input Layer (80 Features)

↓
Dense Layer (100 Neurons, ReLU)

↓
Dropout (0.5)

↓
Dense Layer (200 Neurons, ReLU)

↓
Dropout (0.5)

↓
Dense Layer (100 Neurons, ReLU)

↓
Dropout (0.5)

↓
Output Layer (10 Classes, Softmax)

Training Enhancements:

* Early Stopping
* Model Checkpointing
* Learning Rate Scheduling
* Validation Monitoring

---

## 📊 Evaluation Metrics

The model is evaluated using:

* Accuracy
* Precision
* Recall
* F1 Score
* Confusion Matrix
* Classification Report

---

## 🚀 Results

### Deep Neural Network Performance

| Metric              | Value      |
| ------------------- | ---------- |
| Test Accuracy       | **91.36%** |
| Training Accuracy   | **90.55%** |
| Validation Accuracy | **91.53%** |

### Classification Metrics

* Macro F1 Score: **0.91**
* Weighted F1 Score: **0.91**

---

## 🔍 Model Comparison

| Model                     | Accuracy   |
| ------------------------- | ---------- |
| Deep Neural Network (DNN) | **91.93%** |
| XGBoost                   | 90.27%     |
| Random Forest             | 88.27%     |

The Deep Neural Network achieved the highest accuracy and demonstrated superior generalization capability compared to traditional machine learning models.

---

## 📈 Visualizations

The project includes:

* Confusion Matrix
* Accuracy vs Epoch Plot
* Loss vs Epoch Plot
* Training vs Validation vs Test Accuracy Plot
* Class Distribution Analysis
* Model Accuracy Comparison Chart

---

## 🎵 Custom Audio Prediction

The trained model supports prediction on unseen audio files.

Workflow:

1. Load custom audio file
2. Extract MFCC features
3. Apply feature scaling
4. Generate class probabilities
5. Predict final sound category

Example:

Input Audio: Dog Bark

Predicted Class: Dog Bark ✅

---

## 💡 Applications

* Smart Surveillance Systems
* Environmental Sound Monitoring
* Urban Noise Analysis
* Smart City Infrastructure
* Audio Event Detection
* Security and Public Safety Systems

---

## 📌 Key Learnings

Through this project, I gained hands-on experience in:

* Audio Signal Processing
* Feature Engineering using MFCC
* Deep Learning with TensorFlow/Keras
* Machine Learning Model Comparison
* Hyperparameter Tuning
* Model Evaluation and Visualization
* Real-world Audio Classification Systems

---

## 🔮 Future Improvements

* CNN-based Audio Classification
* Spectrogram-based Deep Learning Models
* Real-time Audio Streaming Classification
* Mobile Deployment
* Transfer Learning Approaches
* Attention-Based Audio Models

---

## 👨‍💻 Author

**Koushal Kishor Vishwakarma**

Electronics and Communication Engineering Student

Interested in Machine Learning, Deep Learning, Signal Processing, and Artificial Intelligence.
