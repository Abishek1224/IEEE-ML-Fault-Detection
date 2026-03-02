# 🔍 Fault Detection using Machine Learning

A machine learning solution for binary fault detection in embedded device systems.

---

## 📖 Project Overview

This project predicts whether a device is operating normally or experiencing a fault condition using 47 numerical features collected from an embedded monitoring system.

- **Class 0 → Normal**
- **Class 1 → Faulty**

This is a binary classification problem.

---

## 📂 Dataset Description

### TRAIN.csv
- 47 input features (F01–F47)
- Target column: `Class`

### TEST.csv
- 47 input features
- `ID` column
- No target column (used for prediction)

---

## ⚙️ Approach

1. Data loaded using pandas
2. Features separated from target variable
3. Model trained using Random Forest Classifier
4. Predictions generated for TEST dataset
5. Final submission file created in required format

---

## 🧠 Model Used

- RandomForestClassifier
- Number of trees: 200
- Random state: 42

---

## 📈 Model Performance

- Basic training validation performed
- Model suitable for binary classification task

---

## 🛠️ Installation & Setup

### Step 1: Install Python (3.x)

### Step 2: Install Required Libraries

```bash
pip install -r requirements.txt
