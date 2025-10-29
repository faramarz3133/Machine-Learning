# 🔢 Dimensionality Reduction and Classification using PCA

## 📘 Overview
This project demonstrates the application of **Principal Component Analysis (PCA)** for dimensionality reduction on the **Digits dataset** and evaluates its effect on classification performance.  
The analysis explores how PCA reduces feature dimensionality while retaining most of the data’s variance, and how this reduction impacts model accuracy and training time.

---

## 📊 Dataset
- **Source:** `sklearn.datasets.load_digits`
- **Samples:** 1,797 handwritten digit images
- **Image Size:** 8 × 8 pixels (64 features)
- **Target Classes:** Digits 0 through 9  
- **Task:** Classify handwritten digits based on their 8×8 grayscale images.

---

## 🔍 Project Workflow

### 1. Data Loading and Exploration
- Loaded dataset using `sklearn.datasets.load_digits(as_frame=True)`
- Separated **features (X)** and **labels (y)**
- Each image represented as a 64-dimensional feature vector (pixel intensities)

### 2. Visualization
- Implemented a helper function to visualize individual digit images  
- Displayed random digit samples to understand data structure

### 3. PCA Analysis
- Performed PCA using all components to compute **explained variance ratio**
- Plotted **explained variance** and **cumulative explained variance**
- Determined the number of principal components required to retain 95% variance
- Found that **29 components** preserve approximately 95% of total variance

### 4. 2D Visualization with PCA
- Reduced data to **2 dimensions** for visualization
- Plotted PCA-transformed points using color-coded labels (0–9)
- Observed clear separability between certain digits (e.g., 0, 1, 7)  
  and overlapping clusters for others (e.g., 3, 8, 9)

### 5. Classification with and without PCA
Two Logistic Regression models were trained and compared:

| Model | Input Features | Components | Accuracy | Training Time |
|--------|----------------|-------------|-----------|----------------|
| **Baseline** | Raw data | 64 | ~0.97 | Higher |
| **PCA Reduced** | PCA-transformed | 29 | ~0.96 | Faster |

#### Key Observations:
- PCA reduced training time significantly while maintaining comparable accuracy.
- Slight loss in precision/recall for a few classes due to minor information loss.
- Dimensionality reduction helps accelerate computation with minimal accuracy tradeoff.

---

## 🧩 Libraries Used
```python
numpy
pandas
matplotlib
scikit-learn
```


## Author
- Faramarz Aghajani
- faramarzaghajani217@gmail.com
- https://github.com/faramarz3133
