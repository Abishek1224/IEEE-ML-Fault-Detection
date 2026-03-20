# 🔍 Fault Detection using Machine Learning

A machine learning solution for binary fault detection in embedded device systems using 47 numerical features.

---

## 📖 Project Overview

This project predicts whether a device is operating normally or experiencing a fault condition based on sensor data.

- **Class 0 → Normal**
- **Class 1 → Faulty**

This is a **binary classification problem**, and evaluation is based on **F1-Score**.

---

## 📂 Dataset Description

### TRAIN.csv
- 47 numerical features (F01–F47)
- Target column: `Class`

### TEST.csv
- 47 numerical features
- `ID` column
- Used for generating predictions

---

## ⚙️ Approach

1. Data loaded using **pandas**
2. Class distribution checked for imbalance
3. Correlation analysis performed using heatmap
4. Features and target separated
5. Data split into training and validation sets (80/20)
6. Model trained using **Random Forest Classifier**
7. Performance evaluated using:
   - Accuracy
   - **F1-Score (Primary metric)**
   - Classification Report
8. Final model retrained on full dataset
9. Predictions generated for TEST dataset

---

## 🌲 Model Used

**RandomForestClassifier**

- n_estimators = 400  
- class_weight = "balanced"  
- random_state = 42  

### Why Random Forest?

- Handles high-dimensional numerical data effectively  
- Reduces overfitting using ensemble learning  
- Works well without heavy feature scaling  
- Robust to noise and suitable for binary classification  

---

## 📈 Model Performance

- Validation Accuracy: ~0.98  
- Validation F1-Score: (add your value here)

The model was evaluated using an 80-20 train-validation split.

---

## 🛠️ Installation & Setup

### Step 1: Install Python (3.x)

### Step 2: Install Required Libraries

```bash
pip install -r requirements.txt
