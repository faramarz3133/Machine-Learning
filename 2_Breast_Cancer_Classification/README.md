# 🧠 Breast Cancer Classification: Predicting Benign vs. Malignant Tumors

## 📘 Overview
This project focuses on building and evaluating machine learning models to classify breast tumors as **benign** or **malignant** using the **Breast Cancer Wisconsin dataset**.  
The workflow includes data exploration, preprocessing, model training, performance evaluation, and hyperparameter optimization using `GridSearchCV`.

---

## 📊 Dataset
- **Source:** `sklearn.datasets.load_breast_cancer`
- **Samples:** 569
- **Features:** 30 numerical features describing tumor properties such as radius, texture, perimeter, area, smoothness, concavity, and more.
- **Target Classes:**
  - `0`: Malignant (Cancerous)
  - `1`: Benign (Non-cancerous)

---

## 🔍 Project Workflow

### 1. Data Loading and Exploration
- Loaded dataset via `sklearn.datasets.load_breast_cancer(as_frame=True)`
- Converted to a Pandas DataFrame
- Explored structure and summary statistics (`info`, `describe`)
- Verified dataset has **no missing values**

### 2. Exploratory Data Analysis (EDA)
- Visualized feature distributions by target class using **Seaborn KDE plots**
- Computed correlation matrix and plotted **heatmaps**
- Identified redundant correlated features and removed them for better interpretability

### 3. Data Preprocessing
- Split the data into **80% training** and **20% testing**
- Standardized features using **StandardScaler**

### 4. Baseline Model
- Trained a **Logistic Regression** classifier as the baseline
- Evaluated using:
  - **Accuracy**
  - **Precision / Recall / F1-score**
  - **Confusion Matrix**

### 5. Model Comparison
Tested and compared multiple classification models:

| Model | Description |
|--------|-------------|
| Logistic Regression | Baseline linear classifier |
| K-Nearest Neighbors (KNN) | Distance-based classification |
| Support Vector Classifier (SVC) | Kernel-based margin classifier |
| Decision Tree | Tree-based model |
| Bagging Classifier | Ensemble of base estimators |
| Random Forest | Ensemble of decision trees |
| Gradient Boosting | Sequential ensemble model |

Each model was trained and evaluated on scaled data using **Accuracy**, **F1-score**, and **Confusion Matrix**.

### 6. Hyperparameter Tuning with GridSearchCV
- Implemented **Pipelines** for standardization and classification
- Performed **GridSearchCV** with:
  - 5-fold cross-validation
  - Scoring: `f1_macro`
  - Parallel execution (`n_jobs=-1`)
- Extracted best hyperparameters and retrained top models
- Summarized results into a comparison DataFrame

---

## 🧩 Libraries Used
```python
pandas
numpy
matplotlib
seaborn
scikit-learn
```


## Author
- Faramarz Aghajani
- faramarzaghajani217@gmail.com
- https://github.com/faramarz3133
