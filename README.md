# Machine-Learning
Collection of my Machine Learning projects including Regression, Classification, Clustering, and PCA

# 🤖 Machine Learning Projects

This repository contains a collection of my **Machine Learning** projects implemented in Python using popular libraries such as **scikit-learn**, **pandas**, **numpy**, and **matplotlib**.  
Each project focuses on a key concept in ML — from **regression** and **classification** to **clustering** and **dimensionality reduction (PCA)**.

---

## 📁 Project Structure


Machine-Learning/
│
├── 1_California_Housing_Price_Prediction/
│ ├── California_Housing_Prediction.ipynb
│ ├── README.md
│ ├── requirements.txt
│
├── 2_Breast_Cancer_Classification/
│ ├── Breast_Cancer_Classification.ipynb
│ ├── README.md
│ └── requirements.txt
│
├── 3_Customer_Segmentation_KMeans/
│ ├── Customer_Segmentation.ipynb
│ ├── README.md
│
└── 4_PCA_Digits_Dataset/
├── PCA_Digits.ipynb
├── README.md

## 🧠 Projects Overview

### 🏠 1. California Housing Price Prediction (Regression)
Predicting California house prices using the `fetch_california_housing` dataset.  
Techniques used:
- Exploratory Data Analysis (EDA)
- Linear Regression & Random Forest
- Model evaluation using R² and RMSE
- Model optimization with **Pipeline + GridSearchCV**

📘 [View Project Folder](./1_California_Housing_Price_Prediction)

---

### 🧬 2. Breast Cancer Classification (Supervised Learning)
Classifying tumors as **Benign** or **Malignant** using the Wisconsin Breast Cancer dataset.  
Key steps:
- Data preprocessing and visualization
- Comparison of multiple classifiers: Logistic Regression, KNN, SVM, Decision Tree, Random Forest, Gradient Boosting
- Model evaluation using Accuracy, F1-Score, Confusion Matrix

📘 [View Project Folder](./2_Breast_Cancer_Classification)

---

### 👥 3. Customer Segmentation using K-Means (Unsupervised Learning)
Segmenting customers based on **Annual Income** and **Spending Score** using **K-Means clustering**.  
Includes:
- Data visualization and correlation analysis
- Finding optimal clusters using the Elbow method
- Visualizing clusters and centroids
- Customer persona interpretation

📘 [View Project Folder](./3_Customer_Segmentation_KMeans)

---

### 🔢 4. PCA on Handwritten Digits Dataset (Dimensionality Reduction)
Applying **Principal Component Analysis (PCA)** to reduce dimensions from 64 → 2 on the Digits dataset.  
Then comparing model performance before and after PCA.  
Includes:
- Explained variance visualization
- 2D scatter plot of PCA components
- Logistic Regression classification
- Comparison of accuracy and training time before/after PCA

📘 [View Project Folder](./4_PCA_Digits_Dataset)

---

## ⚙️ Technologies Used
- Python 🐍  
- pandas, numpy  
- scikit-learn  
- matplotlib, seaborn  
- Jupyter Notebook  

---

## 🚀 How to Run

1. Clone this repository:
   ```bash
   git clone https://github.com/<your-username>/Machine-Learning.git
2.Navigate to any project folder:
    ```bash
    cd Machine-Learning/1_California_Housing_Price_Prediction
3.Install dependencies:
    ```bash
    pip install -r requirements.txt
4.Open the notebook and run all cells:
    ```bash
    jupyter notebook California_Housing_Prediction.ipynb


   
