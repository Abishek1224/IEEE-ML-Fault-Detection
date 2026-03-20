# 🔍 Fault Detection using Machine Learning

## 📖 Project Overview
This project focuses on detecting whether a device is operating under normal conditions or experiencing a fault.  
The classification is performed using 47 numerical features collected from an embedded monitoring system.

- **Class 0 → Normal**
- **Class 1 → Faulty**

This is a binary classification problem.

---

## 📂 Dataset Description

- **TRAIN.csv**
  - 47 input features (F01–F47)
  - Target column: `Class`

- **TEST.csv**
  - 47 input features
  - `ID` column
  - No target column (used for prediction)

---

## ⚙️ Approach

1. Data loaded using **pandas**
2. Features separated from target variable
3. Model trained using **Random Forest Classifier**
4. Predictions generated for TEST dataset
5. Final submission file created in required format

---

## 🧠 Model Used

- RandomForestClassifier  
- Number of trees: 200  
- Random state: 42  

---

## 🛠️ Installation & Setup

### Step 1: Install Python (3.x)

### Step 2: Install Required Libraries

```bash
pip install -r requirements.txt
