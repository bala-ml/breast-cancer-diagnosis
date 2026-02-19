# 🧠 Breast Cancer Prediction using Machine Learning

## 📌 Project Overview

This project focuses on predicting whether a breast cancer tumor is **Benign (B)** or **Malignant (M)** using the Breast Cancer Wisconsin (Diagnostic) Dataset. The dataset contains numerical features extracted from digitized images of Fine Needle Aspirate (FNA) of breast masses, describing characteristics of cell nuclei.

The main objective is to build a reliable classification model with a strong focus on **Recall**, since false negatives (predicting malignant tumors as benign) are critical in medical diagnosis.

---

## 🎯 Problem Statement

Predict whether breast cancer is:

- **M = Malignant**
- **B = Benign**

based on numerical features derived from medical imaging data.

---

## 📊 Dataset Description

**Dataset:** Breast Cancer Wisconsin (Diagnostic) Data Set

Features are computed from digitized images of a fine needle aspirate (FNA) of a breast mass. They describe characteristics of the cell nuclei present in the image.

📎 Dataset Source:  
https://archive.ics.uci.edu/ml/datasets/Breast+Cancer+Wisconsin+%28Diagnostic%29

Original Research Reference:  
K. P. Bennett and O. L. Mangasarian (1992) – Robust Linear Programming Discrimination of Two Linearly Inseparable Sets.

---

## 🧾 Attribute Information

1. ID Number
2. Diagnosis (Target Variable)
3–32. Thirty real-valued features derived from ten core measurements:

### 🔬 Core Features

- Radius – mean distance from center to perimeter points
- Texture – standard deviation of gray-scale values
- Perimeter
- Area
- Smoothness – local variation in radius lengths
- Compactness – perimeter² / area − 1.0
- Concavity – severity of concave portions
- Concave Points – number of concave regions
- Symmetry
- Fractal Dimension – coastline approximation

For each image, the following were computed:

- Mean values
- Standard Error (SE)
- Worst (largest values)

Total Features: **30 numerical features**

---

## 📈 Dataset Insights

- ID column removed (not useful for prediction)
- All features are numerical (no categorical variables)
- High-dimensional feature space
- No missing values
- Slight class imbalance:
  - 357 Benign
  - 212 Malignant
- Recall is prioritized as the main evaluation metric
- Strong separation in feature means between classes
- Extreme values often represent malignant cases (not noise)
- Highly correlated features present → PCA or Feature Selection recommended

---

## ⚙️ Tech Stack

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn

---

## 🔄 Machine Learning Pipeline

1. Data Cleaning & Preprocessing
2. Exploratory Data Analysis (EDA)
3. Data Visualization
4. Feature Scaling using StandardScaler
5. Train-Test Split
6. Model Training (Support Vector Machine / Classification Model)
7. Model Evaluation

---

## 📊 Evaluation Metrics

Since false negatives are critical:

- Recall Score (Primary Metric)
- Precision
- Accuracy
- Confusion Matrix

---

## 📂 Project Structure

├── data/
├── notebooks/
├── src/
├── requirements.txt
└── README.md

---

## 📂 Project Structure

```
breast-cancer-diagnosisn-ml/
│
├── data/
│   └── breast_cancer.csv
│
├── notebook/
│   └── breast_cancer_diagnosis.ipynb
│
├── requirements.txt
└── README.md
```

---

## ▶️ How to Run the Project

### 1️⃣ Clone the Repository

```
git clone origin https://github.com/bala-ml/breast-cancer-diagnosis.git
```

### 2️⃣ Install Dependencies

```
pip install -r requirements.txt
```

### 3️⃣ Run the Notebook

Open the Jupyter Notebook and execute all cells.

---

## 💡 Future Improvements

- Apply PCA for dimensionality reduction
- Feature selection to reduce multicollinearity
- Hyperparameter tuning
- Compare multiple machine learning models

---

## 👤 Author

    Balaji I
    🎯 Aspiring Machine Learning Engineer
    📍 India

---