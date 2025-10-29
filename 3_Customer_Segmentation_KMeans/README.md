# 🛍️ Customer Clustering Using K-Means

## 📘 Overview
This project performs **customer clustering** using the **K-Means clustering algorithm** on the *Mall Customers Dataset*.  
The goal is to group customers into distinct clusters based on their **annual income** and **spending score**, helping businesses understand different spending behaviors and design targeted marketing strategies.

---

## 📊 Dataset
- **Dataset Name:** `Mall_Customers.csv`
- **Source:** Public dataset available on Kaggle and other educational repositories.
- **Records:** 200 customers
- **Features:**
  - `CustomerID`: Unique identifier for each customer  
  - `Gender`: Male or Female  
  - `Age`: Age of the customer  
  - `Annual Income (k$)`: Annual income in thousands of dollars  
  - `Spending Score (1–100)`: Spending score assigned by the mall based on customer behavior

---

## 🔍 Project Workflow

### 1. Data Loading and Cleaning
- Imported dataset using **Pandas**
- Encoded categorical features (Gender) using `pd.get_dummies()`
- Removed the non-informative column `CustomerID`
- Renamed columns for clarity:
  - `Annual Income (k$)` → `Income`
  - `Spending Score (1-100)` → `Score`

### 2. Exploratory Data Analysis (EDA)
- Analyzed gender distribution through **bar plots**
- Visualized feature distributions (Age, Income, Spending Score) using **KDE plots**
- Explored pairwise feature relationships using **Seaborn pairplots**
- Visualized feature correlations via **heatmaps**
- Observed clear clustering tendencies in the *Income vs Spending Score* space

### 3. Data Preprocessing
- Selected relevant features for clustering: `Income` and `Score`
- Standardized numerical values using **StandardScaler** for fair distance computation

### 4. Determining Optimal Number of Clusters
- Applied the **Elbow Method** to analyze Within-Cluster Sum of Squares (WCSS)
- Selected **K = 5** as the optimal number of clusters based on elbow curve behavior

### 5. Model Training
- Built and trained **KMeans** model (`n_clusters=5`, `random_state=42`)
- Assigned each customer to one of five clusters
- Calculated and visualized cluster centroids (in inverse-scaled units)

### 6. Visualization and Insights
- **Scatter Plot:** Income vs Spending Score colored by cluster labels
- **Centroids:** Displayed as red stars to mark cluster centers
- **Gender Distribution:** Bar chart showing male/female ratio per cluster
- **Cluster Analysis:** Computed average metrics per cluster (Age, Income, Spending Score)

---

## 📈 Results Summary

| Cluster | Profile Description | Characteristics |
|----------|---------------------|-----------------|
| 0 | **Cautious Spenders** | Low income, low spending |
| 1 | **Target Customers** | High income, high spending |
| 2 | **Moderate Buyers** | Mid-range income and spending |
| 3 | **Young & Lavish** | Lower income, high spending score |
| 4 | **Savers** | Low spending despite moderate income |

These clusters provide actionable insights for customer segmentation and personalized marketing strategies.

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
